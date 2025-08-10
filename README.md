# Standardized Soil Moisture Index using Python API (Xee)
## Overview
This project performs a spatiotemporal analysis of soil moisture anomalies using NASA SMAP (Soil Moisture Active Passive) data from 2016 to 2024.

The script leverages Google Earth Engine (GEE), geemap, and xarray to:
1. Retrieve monthly soil moisture data for a selected region of interest (ROI).
2. Compute the Soil Moisture Standardized Index (SSI) based on historical mean and standard deviation.
3. Generate visualizations of soil moisture anomalies at different time scales.
4. Export spatial plots for reporting and further analysis.

## Key Features
<img width="608" height="110" alt="image" src="https://github.com/user-attachments/assets/6ec6355f-9799-4ceb-b619-64bfa614a162" />

### Long-Term Mean Soil Moisture (2016–2024)
<img width="571" height="432" alt="image" src="https://github.com/user-attachments/assets/ec8901ce-e4ad-4f82-a39b-4eb9f06758c8" />

### Long-Term Standard Deviation of Soil Moisture (2016–2024)
<img width="571" height="432" alt="image" src="https://github.com/user-attachments/assets/99b251b1-bbda-4a8b-b7f1-b5b2fb704ef9" />

### Long-Term Standard Deviation of Soil Moisture (2016–2024)
<img width="1182" height="590" alt="image" src="https://github.com/user-attachments/assets/f99a9f15-db10-4d00-b44c-2ab94d9bfef5" />

### Monthly Standardized Soil Moisture Index (SSI) for 2019
<img width="1197" height="889" alt="image" src="https://github.com/user-attachments/assets/d56db454-4178-4850-b452-6379184a8de3" />


## Notes
1. This script requires a valid GEE account with high-volume API access (https://earthengine-highvolume.googleapis.com) and should be run in an environment that supports interactive map drawing.
2.  Users should ensure that the ROI size is reasonable to avoid large data requests that may cause processing delays.
3.  All computations are done in EPSG:4326 (WGS 84) coordinate reference system, and plots are generated with robust scaling for better contrast.
