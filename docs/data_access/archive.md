---
title: Archive
layout: default
parent: Data access
---

# Archive

Data is archived in separate \*.parquet files for each device and hour.
The path of each blob strictly follows the following format:
`archive/device={device}/year={year:04d}/month={month:02d}/day={day:02d}/hour={hour:02d}/creation_time_seconds.parquet`


## Azure SDK (Python)
> Please, consult [official Azure SDK for Python documentation](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) for more details.

At least the following operations are necessary to access data:

- [List blobs](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) with prefix
- [Download blob](https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blob-download-python)


(pseudo)code example to list and download blobs for device test-001 with data from January 2026:
```
from azure.storage.blob import BlobServiceClient, ContainerClient
import pandas as pd
from io import BytesIO


CONTAINER_NAME = "..."
CONNECTION_STRING = "secret"
BLOB_PREFIX = "archive/device=test-001/year=2026/month=01/"

blob_service = BlobServiceClient.from_connection_string(CONNECTION_STRING)
container_client = blob_service.get_container_client(CONTAINER_NAME)

# 1. list blobs
blobs = container_client.list_blobs(name_starts_with=BLOB_PREFIX)

# 2. download blobs into pandas dataframes
dfs = []
    for blob in blobs:
        blob_client = container_client.get_blob_client(blob)
        stream = blob_client.download_blob()
        data = stream.readall()
        dfs.append(
            pd.pd.read_parquet(
                BytesIO(data)
            )
        )
# use own logic to merge dfs to single df if needed
```

> **Note:** Some hours per device might have data split in multiple blobs - this happens if part of data for specific hour and device arrives with a delay, once original batch had been processed. Own logic should be used to merge those in desired way or in some cases the more recent file can be ignored. Strategies at the data collection side will be put in place to minimise the occurance of these cases.
> Please, alway expect multiple blobs to be processed and merge them into single dataframe. Use `timestamp` as index.
>
> The following pseudo code (Python + Azure SDK + Pandas) might help:
> ```
> blobs = container_client.list_blobs(name_starts_with=parquet_blob_name_prefix)
> dfs = []
>    for blob in blobs:
>        blob_client = container_client.get_blob_client(blob)
>        stream = blob_client.download_blob()
>        data = stream.readall()
>        dfs.append(
>            pd.read_parquet(
>                BytesIO(data),
>                parse_dates=["timestamp"],
>                index_col="timestamp",
>                engine="pyarrow"
>            ).groupby(level=0).last()
>        )
>
>    df = (
>        pd.concat(dfs)
>        .groupby(level=0)
>        .last()
>        .sort_index()
>    )
>    ```



> More example scripts can be found in [Github repository](https://github.com/IdealAQ/aq-data-az-blob).