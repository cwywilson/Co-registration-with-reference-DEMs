# DEM Co-Registration and Glacier Change Detection in Auyuittuq and Sirmilik National Parks

This repository provides workflows and code for co-registering historical and modern Digital Elevation Models (DEMs), and for quantifying glacier surface elevation and volume changes in the Canadian Arctic. The focus areas are **Auyuittuq National Park (ANP)** and **Sirmilik National Park (SNP)**, where long-term glacier monitoring is essential for understanding climate-driven cryospheric change.

## Repository Contents

* **`SNP DEM coregister.ipynb`**
This notebook demonstrates the co-registration of a 1958 historical DEM to a reference ArcticDEM mosaic (2022) using the [`xdem`](https://github.com/GlacioHack/xdem) library.  
Key steps include:
- Loading and reprojecting input DEMs
- Handling nodata values and filtering erroneous elevations
- Visualizing spatial extent and glacier outlines
- Performing co-registration using bias correction methods
- Evaluating co-registration performance through residual analysis and plots

* **`ANP DEM difference.ipynb`**  
  This notebook performs elevation differencing between co-registered DEMs to assess glacier surface elevation change from the 1959 historical DEM to the 2021/22 ArcticDEM strip. Key steps include:

  * Reprojecting DEMs and handling nodata values
  * Applying slope and glacier masks to isolate stable terrain and glacierized areas
  * Performing DEM co-registration (if needed)
  * Estimating elevation uncertainty
  * Visualizing and exporting elevation difference maps


## Acknowledgements

* [XDEM Team](https://github.com/GlacioHack/xdem)

