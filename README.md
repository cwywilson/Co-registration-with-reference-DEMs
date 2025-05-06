# DEM Co-Registration and Glacier Change Detection in SNP and ANP

This repository contains code and workflows for co-registering historical and modern Digital Elevation Models (DEMs), and computing glacier elevation change and volume change in the Canadian Arctic, particularly in Auyuittuq National Park (ANP) and Sirmilik National Park (SNP).

## Repository Contents

* **`SNP DEM coregister.ipynb`**
  This notebook aligns a historical 1958 DEM to a reference ArcticDEM (2022) using the [XDEM](https://github.com/GlacioHack/xdem) library. Steps include:

  * Reading and reprojecting DEMs
  * Setting nodata values and cleaning erroneous elevations
  * Visualizing extent and preparing for co-registration
  * Performing co-registration 
  * Evaluating residuals between DEMs before and after alignment

* **`ANP DEM difference.ipynb`**
  This notebook performs elevation differencing between the co-registered DEMs to assess glacier surface change from 1959 to 2021/22. It includes:

  * Reprojection and nodata setup
  * DEM differencing and masking
  * Uncertainty estimation
  * Plotting elevation difference maps
  * Exporting geotiffs and summary statistics


## Acknowledgements

* [XDEM Team](https://github.com/GlacioHack/xdem)

