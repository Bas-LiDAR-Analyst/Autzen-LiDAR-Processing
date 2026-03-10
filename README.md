# Autzen LiDAR Data Processing Pipeline

This project demonstrates a complete LiDAR data processing workflow to generate a Digital Elevation Model (DEM).

## Overview
- **Data Source:** Autzen Stadium LiDAR Point Cloud.
- **Tools Used:** PDAL, QGIS, CloudCompare.
- **Output:** 1-meter resolution DEM with Hillshade and Contour analysis.

## Workflow Summary
1. **Ground Classification:** Used PDAL `filters.smrf` to isolate ground points from the point cloud.
2. **Rasterization:** Created a high-resolution DEM using the `writers.gdal` driver.
3. **Visualization:** Stylized in QGIS using:
    - **Singleband Pseudocolor:** For elevation-based coloring.
    - **Hillshade:** For 3D terrain visualization.
    - **Contour Extraction:** 1-meter interval lines for topographic study.

## Files in this Repository
- `create_dem.json`: The PDAL pipeline used for processing.
- `Autzen_dem.pdf`: The final professional map layout.
