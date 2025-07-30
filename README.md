# Glacier Elevation Change Detection via DEM Co-Registration in Auyuittuq and Sirmilik National Parks

This repository provides workflows and code for co-registering historical and modern Digital Elevation Models (DEMs) using the [`xdem`](https://github.com/GlacioHack/xdem) library, and for quantifying glacier surface elevation and volume changes in the Canadian Arctic. The focus areas are **Auyuittuq National Park (ANP)** and **Sirmilik National Park (SNP)**, where long-term glacier monitoring is essential for understanding climate-driven cryospheric change.

## 📂 Repository Structure

| File | Purpose |
|------|---------|
| `SNP DEM coregister.ipynb` | Co-registers and computes elevation differences between a 1958 historical DEM and 2022 ArcticDEM for Sirmilik National Park (SNP).|
| `ANP DEM difference.ipynb` | Co-registers and computes elevation differences between a 1959 historical DEM and 2021/22 ArcticDEM for Auyuittuq National Park (ANP). |

## ⚙️ Features

- DEM Preprocessing and Reprojection
Ensures consistent projection, resolution, and nodata handling across historical and modern DEMs.

- Glacier and Terrain Masking
Applies glacier outlines and slope thresholds to isolate stable terrain and glacier-covered areas for accurate differencing.

- Robust Co-registration
Uses xdem-based Deramp and NuthKaab methods to align historical DEMs with modern ArcticDEM strips, correcting for tilt, bias, and distortion.

- Elevation Change and Uncertainty Estimation
Computes elevation differences (Δh), estimates uncertainties using NMAD over stable terrain.

- Visualization
Produces clear elevation change maps, slope masks, residual plots, and histograms to support data validation and interpretation.

## 🧪 Sample Outputs

- Glacier elevation change maps
- Residual error statistics
- Plots of vertical bias vs terrain features

## Acknowledgements

* [XDEM Team](https://github.com/GlacioHack/xdem)

