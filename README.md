## Sathwik Ramaka

M.Sc. Agriculture Analytics — a joint programme across DAU Gandhinagar, **IIRS-ISRO Dehradun**, and Anand Agricultural University. I build machine learning pipelines on satellite imagery for soil, crop, and land-use problems.

Available January–June 2027 for a six-month research internship (mandatory curriculum placement).

---

### Projects

**[Regional Carbon Stock Intelligence System](https://github.com/sathwikramaka/carbon-stock-estimation-ludhiana)** — Ludhiana, Punjab
Soil organic carbon across a 64,545-cell, 250 m grid: 5.09 MtC (0–30 cm), with above-ground assimilation reported separately as an annual flux rather than summed with it.
The part worth reading is the validation. Inputs were audited against published ranges for Punjab soils, which surfaced a unit-scaling error that had the district estimate off by 10×. Random splits were replaced with spatial block cross-validation. Every predictor was tested for reconstructability from coordinates alone — four climate covariates came back above R² 0.96 from latitude and longitude, meaning they were acting as positional proxies rather than physical drivers. The README states plainly which of the two reported R² values is trustworthy and why the other is not.
Team project (SpatioFarm, four members). My role: the ML pipeline, the Flask REST API, and the dashboard front end.
`Python` `scikit-learn` `Google Earth Engine` `PostGIS` `Flask` `Leaflet.js` `MongoDB`

**[Agrivoltaic Site Suitability Optimiser](https://github.com/sathwikramaka/agrivoltaic-site-optimizer-jodhpur)** — Jodhpur, Rajasthan
Ranked land for combined solar and agricultural use across 47.6 million pixels using multi-criteria decision analysis over six weighted criteria plus K-means clustering. The raster stage was GPU-accelerated with PyTorch tensor operations on CUDA, which made full-district runs fast enough to iterate on.
Team project (SpatioFarm, four members). My role: ML and spatial analysis.
`Python` `rasterio` `geopandas` `scikit-learn` `PyTorch/CUDA`

**[FasalAlert](https://github.com/SpatioFarm/fasalalert)** — pan-India crop stress advisory
Real-time crop stress scoring from weather anomalies against IMD climate normals and the ICAR crop calendar, rendered as an interactive district choropleth.
Team project (SpatioFarm, four members). My role: the Streamlit dashboard (`app.py`).
`Python` `Streamlit` `GeoPandas` `Folium` `OpenWeatherMap API`

**[Soil Organic Carbon Mapping](https://github.com/sathwikramaka/soil-carbon-mapping-uttarakhand)** — Dhanolti, Uttarakhand
Topsoil SOC over mountainous terrain, Random Forest on 27 Google Earth Engine covariates structured on the SCORPAN-E soil-forming-factor framework. Outputs a prediction raster plus an uncertainty raster derived from the spread across trees.
R² 0.44 under random k-fold. Written in R, co-authored with K. Yaswanthi.
`R` `randomForest` `caret` `terra` `sf` `Google Earth Engine`

---

### Stack

Where I actually am, not where I'd like to be:

| | |
|---|---|
| **Work independently** | Python, Google Earth Engine, pandas, NumPy, scikit-learn, GeoPandas, Rasterio, QGIS, PostGIS, Flask, Git |
| **Working knowledge** | R, SQL, Sentinel-1/2, Landsat, MODIS, spectral indices, spatial cross-validation, leakage and proxy diagnostics |
| **Learning now** | PyTorch for network training (so far I have used it as a GPU array backend, not for deep learning), semantic segmentation on multispectral imagery, xarray/rioxarray |

---

### Certifications

NASA ARSET — Fundamentals of Remote Sensing (Jan 2026)
NASA ARSET — Hyperspectral Data for Land and Coastal Systems (Jan 2026)

---

sathvikramaka@gmail.com · [LinkedIn](https://www.linkedin.com/in/sathwik-ramaka-1ba40227a/)
