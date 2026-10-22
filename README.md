# Krishna–Budameru Flood Mapping and Terrain Analysis

A Google Earth Engine project for estimating flood inundation and
analysing terrain, vegetation, and surface water in a rectangular
study area around Vijayawada, Andhra Pradesh, India.

## Project status

Satellite-analysis outputs have been exported.
Flood-map validation and final map preparation are pending.
An operational early-warning system is not implemented.

## Objectives

- Estimate potential inundation using Sentinel-1 SAR change detection.
- Analyse elevation and slope using SRTM DEM.
- Calculate vegetation conditions using Sentinel-2 NDVI.
- Calculate surface-water indicators using Sentinel-2 NDWI.

## Study area

The analysis uses a rectangular region of interest:

- Longitude: 80.52° E to 80.85° E
- Latitude: 16.50° N to 16.85° N

This rectangle is an analysis boundary, not a delineated
Krishna or Budameru catchment boundary.

## Datasets

- Sentinel-1 GRD: COPERNICUS/S1_GRD
- Sentinel-2 surface reflectance: COPERNICUS/S2_SR_HARMONIZED
- SRTM DEM: USGS/SRTMGL1_003

Additional datasets and exact processing parameters are documented
in the scripts and methodology.

## Scripts

- scripts/01_flood_terrain_water_analysis.js
- scripts/02_ndvi_fixed.js

## Outputs

- Estimated flood extent
- Elevation
- Slope
- NDVI
- NDWI
- NDWI-based water mask

## How to run

1. Open Google Earth Engine Code Editor.
2. Copy one of the JavaScript scripts into a new file.
3. Review the study area, dates, and processing parameters.
4. Run the script and inspect the Console and map.
5. Run the required export tasks from the Tasks panel.
6. Repeat for the separate NDVI script.

## Limitations

- SAR-derived inundation is an estimate, not ground truth.
- Thresholds require validation.
- Clouds can leave gaps in Sentinel-2 outputs.
- Multi-date composites do not necessarily represent peak flooding.
- NDVI and NDWI alone do not constitute a flood-risk assessment.
- Forecasting and operational alerts are not implemented.

## Future work

- Validate estimated inundation against independent reference data.
- Add population and infrastructure exposure analysis.
- Add rainfall and water-level observations.
- Develop and validate an early-warning prototype.

## Author

Your Name
M.Tech student, Andhra University
