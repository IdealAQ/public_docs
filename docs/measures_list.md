---
title: Measures list
layout: default
nav_order: 2
---

# Measures

The measure key follows the following pattern: **\<sensor\>\_\<measure\>\_\<unit\>**

## Units

| unit | description |
|------|------------|
| ppm | parts per million |
| ppb | parts per billion |
| pct | percent |
| db | decibels |
| c | Celsius |
| ugm3 | micrograms per m3 |
| ptcm3 | particle concentration per cm3 |
| nm | nanometer |
| um2cm3 | square micrometers per cubic centimeter |
| dd | decimal degree |
| hpa | hPa | hectopascal |
| x | unknown |
| xx | unknown |

## List

> **Note:** Not all measures and their values are verified or contain useful value. The presence of all keys listed below in the data is not guaranteed.

Every data item is expected to contain **timestamp** key-value pair, used as index.

| sensor | measure | unit | key | note |
|--------|----------|------|------|------|
| *AirSENCE* | *deviceaddress* | *xx* | *airsence_deviceaddress_xx* | not validated – do not use |
| *AirSENCE* | *baudrate* | *xx* | *airsence_baudrate_xx* | not validated – do not use |
| *AirSENCE* | *dataformat* | *xx* | *airsence_dataformat_xx* | not validated – do not use |
| **AirSENCE** | **co** | **ppb** | **airsence_co_ppb** | |
| **AirSENCE** | **no** | **ppb** | **airsence_no_ppb** | |
| **AirSENCE** | **no2** | **ppb** | **airsence_no2_ppb** | |
| **AirSENCE** | **o3** | **ppb** | **airsence_o3_ppb** | |
| **AirSENCE** | **so2** | **ppb** | **airsence_so2_ppb** | |
| **AirSENCE** | **h2s** | **ppb** | **airsence_h2s_ppb** | |
| **AirSENCE** | **co2** | **ppm** | **airsence_co2_ppm** | |
| **AirSENCE** | **voc** | **ppm** | **airsence_voc_ppm** | |
| **AirSENCE** | **nh3** | **ppm** | **airsence_nh3_ppm** | |
| **AirSENCE** | **ch4** | **ppm** | **airsence_ch4_ppm** | |
| **AirSENCE** | **tempob** | **c** | **airsence_tempob_c** | |
| **AirSENCE** | **humob** | **pct** | **airsence_humob_pct** | |
| **AirSENCE** | **pressureob** | **x** | **airsence_pressureob_x** | |
| **AirSENCE** | **tempamb** | **x** | **airsence_tempamb_x** | |
| **AirSENCE** | **humamb** | **x** | **airsence_humamb_x** | |
| **AirSENCE** | **pressureamb** | **x** | **airsence_pressureamb_x** | |
| *AirSENCE* | *pm1p0* | *xx* | *airsence_pm1p0_xx* | not validated – do not use |
| *AirSENCE* | *pm2p5* | *xx* | *airsence_pm2p5_xx* | not validated – do not use |
| *AirSENCE* | *pm10* | *xx* | *airsence_pm10p0_xx* | not validated – do not use |
| *AirSENCE* | *pm4* | *xx* | *airsence_pm4p0_xx* | not validated – do not use |
| **AirSENCE** | **noiseleq** | **db** | **airsence_noiseleq_db** | |
| **AirSENCE** | **noisemax** | **db** | **airsence_noisemax_db** | |
| *AirSENCE* | *windgust* | *xx* | *airsence_windgust_xx* | not validated – do not use |
| *AirSENCE* | *windspeed* | *xx* | *airsence_windspeed_xx* | not validated – do not use |
| *AirSENCE* | *winddirection* | *xx* | *airsence_winddirection_xx* | not validated – do not use |
| *AirSENCE* | *rainfall* | *xx* | *airsence_rainfall_xx* | not validated – do not use |
| *AirSENCE* | *lux* | *xx* | *airsence_lux_xx* | not validated – do not use |
| *AirSENCE* | *uv* | *xx* | *airsence_uv_xx* | not validated – do not use |
| *AirSENCE* | *lat* | *xx* | *airsence_lat_xx* | not validated – do not use |
| *AirSENCE* | *long* | *xx* | *airsence_long_xx* | not validated – do not use |
| *AirSENCE* | *elev* | *xx* | *airsence_elev_xx* | not validated – do not use |
| *AirSENCE* | *aqiaqhi* | *xx* | *airsence_aqiaqhi_xx* | not validated – do not use |
| **Alphasense OPC** | **temp** | **c** | **alphopc_temp_c** | |
| **Alphasense OPC** | **rh** | **pct** | **alphopc_rh_pct** | |
| **Alphasense OPC** | **pm1** | **ugm3** | **alphopc_pm1p0_ugm3** | |
| **Alphasense OPC** | **pm2p5** | **ugm3** | **alphopc_pm2p5_ugm3** | |
| **Alphasense OPC** | **pm10** | **ugm3** | **alphopc_pm10p0_ugm3** | |
| **naneos** | **pnc** | **ptcm3** | **naneos_pnc_ptcm3** | |
| **naneos** | **diameter** | **nm** | **naneos_diameter_nm** | |
| **naneos** | **ldsa** | **um2cm3** | **naneos_ldsa_um2cm3** | |
| *naneos* | *totalsurfacearea* | *xx* | *naneos_totalsurfacearea_xx* | not validated – do not use |
| **naneos** | **pm2p5** | **ugm3** | **naneos_pm2p5_ugm3** | |
| *naneos* | *geomstddev* | *xx* | *naneos_geomstddev_xx* | not validated – do not use |
| *naneos* | *chargerdiffusioncurrent* | *xx* | *naneos_chargerdiffusioncurrent_xx* | not validated – do not use |
| *naneos* | *chargerhighvoltage* | *xx* | *naneos_chargerhighvoltage_xx* | not validated – do not use |
| *naneos* | *precipitatorvoltage* | *xx* | *naneos_precipitatorvoltage_xx* | not validated – do not use |
| *naneos* | *flow* | *xx* | *naneos_flow_xx* | not validated – do not use |
| *naneos* | *batteryvoltage* | *xx* | *naneos_batteryvoltage_xx* | not validated – do not use |
| *naneos* | *pumpcurrent* | *xx* | *naneos_pumpcurrent_xx* | not validated – do not use |
| *naneos* | *status* | *xx* | *naneos_status_xx* | not validated – do not use |
| *naneos* | *solutionsteps* | *xx* | *naneos_solutionsteps_xx* | not validated – do not use |
| *naneos* | *dNdlogD1* | *xx* | *naneos_dNdlogD1_xx* | not validated – do not use |
| *naneos* | *dNdlogD2* | *xx* | *naneos_dNdlogD2_xx* | not validated – do not use |
| *naneos* | *dNdlogD3* | *xx* | *naneos_dNdlogD3_xx* | not validated – do not use |
| *naneos* | *dNdlogD4* | *xx* | *naneos_dNdlogD4_xx* | not validated – do not use |
| *naneos* | *dNdlogD5* | *xx* | *naneos_dNdlogD5_xx* | not validated – do not use |
| *naneos* | *dNdlogD6* | *xx* | *naneos_dNdlogD6_xx* | not validated – do not use |
| *naneos* | *dNdlogD7* | *xx* | *naneos_dNdlogD7_xx* | not validated – do not use |
| *naneos* | *dNdlogD8* | *xx* | *naneos_dNdlogD8_xx* | not validated – do not use |
| **nsrtmk4** | **noisemax** | **db** | **nsrtmk4_noisemax_db** | |
| **nsrtmk4** | **noiseleq** | **db** | **nsrtmk4_noiseleq_db** | |
| **dashboard** | **GPS latitude** | dd | **dash_lat_dd** | |
| **dashboard** | **GPS longitude** | dd | **dash_long_dd** | |
| **Particles Plus** | **pm2p5** | **ugm3** | **pplus_pm2p5_ugm3** | |
| **Particles Plus** | **pm10** | **ugm3** | **pplus_pm10_ugm3** | |
| **Particles Plus** | **pnc** | **ptcm3** | **pplus_pnc_ptcm3** | |
| **Particles Plus** | **dNdlogdP300to350nm** | **ptcm3** | **pplus_dNdlogdP300to350nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP350to400nm** | **ptcm3** | **pplus_dNdlogdP350to400nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP400to450nm** | **ptcm3** | **pplus_dNdlogdP400to450nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP450to500nm** | **ptcm3** | **pplus_dNdlogdP450to500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP500to550nm** | **ptcm3** | **pplus_dNdlogdP500to550nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP550to600nm** | **ptcm3** | **pplus_dNdlogdP550to600nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP600to650nm** | **ptcm3** | **pplus_dNdlogdP600to650nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP650to700nm** | **ptcm3** | **pplus_dNdlogdP650to700nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP700to800nm** | **ptcm3** | **pplus_dNdlogdP700to800nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP800to900nm** | **ptcm3** | **pplus_dNdlogdP800to900nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP900to1000nm** | **ptcm3** | **pplus_dNdlogdP900to1000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP1000to1250nm** | **ptcm3** | **pplus_dNdlogdP1000to1250nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP1250to1500nm** | **ptcm3** | **pplus_dNdlogdP1250to1500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP1500to2000nm** | **ptcm3** | **pplus_dNdlogdP1500to2000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP2000to2500nm** | **ptcm3** | **pplus_dNdlogdP2000to2500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP2500to3000nm** | **ptcm3** | **pplus_dNdlogdP2500to3000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP3000to3500nm** | **ptcm3** | **pplus_dNdlogdP3000to3500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP3500to4000nm** | **ptcm3** | **pplus_dNdlogdP3500to4000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP4000to4500nm** | **ptcm3** | **pplus_dNdlogdP4000to4500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP4500to5000nm** | **ptcm3** | **pplus_dNdlogdP4500to5000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP5000to5500nm** | **ptcm3** | **pplus_dNdlogdP5000to5500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP5500to6000nm** | **ptcm3** | **pplus_dNdlogdP5500to6000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP6000to6500nm** | **ptcm3** | **pplus_dNdlogdP6000to6500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP6500to7000nm** | **ptcm3** | **pplus_dNdlogdP6500to7000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP7000to7500nm** | **ptcm3** | **pplus_dNdlogdP7000to7500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP7500to8000nm** | **ptcm3** | **pplus_dNdlogdP7500to8000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP8000to8500nm** | **ptcm3** | **pplus_dNdlogdP8000to8500nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP8500to9250nm** | **ptcm3** | **pplus_dNdlogdP8500to9250nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP9250to10000nm** | **ptcm3** | **pplus_dNdlogdP9250to10000nm_ptcm3** | |
| **Particles Plus** | **dNdlogdP10000to25000nm** | **ptcm3** | **pplus_dNdlogdP10000to25000nm_ptcm3** | |
| **hdc3022** | **temperature** | **c** | **hdc3022_temp_c** | |
| **hdc3022** | **humidity** | **pct** | **hdc3022_rh_pct** | |