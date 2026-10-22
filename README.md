# Krishna–Budameru Flood Mapping and Terrain Analysis

A satellite-based geospatial project for estimating flood inundation
and analysing terrain, vegetation, and surface water around
Vijayawada, Andhra Pradesh, using Google Earth Engine.

## Objectives

- Estimate flood inundation using Sentinel-1 SAR imagery.
- Analyse elevation and slope using SRTM DEM.
- Calculate NDVI to examine vegetation conditions.
- Calculate NDWI to identify potential surface-water areas.
- Export analysis results for further mapping and validation.

## Study Area

The project uses a rectangular region of interest around Vijayawada:

- Longitude: 80.52° E to 80.85° E
- Latitude: 16.50° N to 16.85° N

This rectangle is the satellite-analysis boundary.
It is not a delineated Krishna or Budameru catchment boundary.

## Data Used

| Dataset | Purpose |
|---------|---------|
| Sentinel-1 GRD | SAR-based flood estimation |
| Sentinel-2 Surface Reflectance | NDVI and NDWI analysis |
| SRTM DEM | Elevation and slope analysis |

See the published scripts for exact dates, filters, thresholds,
and any additional datasets used.

## Tools Used

- Google Earth Engine
- JavaScript

## Methodology

1. Define the study-area boundary.
2. Select Sentinel-1 imagery before and during the flood period.
3. Compare VV backscatter to identify potential inundation.
4. Apply the water-exclusion method documented in the script.
5. Generate elevation and slope layers from SRTM DEM.
6. Calculate NDVI and NDWI using Sentinel-2 imagery.
7. Export the results as GeoTIFF files.

## Exported Outputs

- Krishna_Budameru_DEM.tif
- Krishna_Budameru_Flood_Extent_2024.tif
- Krishna_Budameru_NDVI_FIXED_2024.tif
- Krishna_Budameru_NDWI_2024.tif
- Krishna_Budameru_NDWI_Water_Mask_2024.tif
- Krishna_Budameru_Slope.tif

## Code

The working Google Earth Engine scripts will be stored in:

- scripts/01_flood_terrain_water_analysis.js
- scripts/02_ndvi_fixed.js

## How to Run

1. Sign in to Google Earth Engine Code Editor.
2. Copy a published JavaScript script into a new script.
3. Review the study area and processing parameters.
4. Run the script.
5. Inspect the Console and map layers.
6. Start the required exports from the Tasks panel.
7. Download the exported files from Google Drive.

## Project Status

- Satellite-analysis outputs exported.
- Final cartographic maps and independent validation pending.
- Early-warning functionality is planned, not implemented.

## Limitations

- The flood layer represents estimated inundation, not ground truth.
- Detection thresholds require independent validation.
- Clouds can limit usable Sentinel-2 observations.
- Multi-date composites may not represent peak flood conditions.
- Flood mapping alone is not a complete flood-risk assessment.

## Future Work

- Validate flood extent using independent reference data.
- Assess population and infrastructure exposure.
- Integrate rainfall and water-level observations.
- Develop and validate an early-warning prototype.

## Author

Amulya k 
M.Tech, Andhra University
