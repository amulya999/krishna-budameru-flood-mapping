<img width="942" height="670" alt="NDWI" src="https://github.com/user-attachments/assets/73a747e3-ad58-4917-9306-73f23f0ddb52" />
<img width="1001" height="705" alt="DEM modified" src="https://github.com/user-attachments/assets/20e6bcd5-a6ca-4d11-95fb-bfa3f2c33870" />
<img width="1122" height="794" alt="SLOPE" src="https://github.com/user-attachments/assets/e29098de-b617-4b00-82ae-42593295ec12" />
# Data Sources and Exported Outputs

## Earth Engine datasets

- Sentinel-1 GRD: COPERNICUS/S1_GRD
- Sentinel-2 surface reflectance: COPERNICUS/S2_SR_HARMONIZED
- SRTM DEM: USGS/SRTMGL1_003

If used by the published script:
- JRC Global Surface Water: JRC/GSW1_4/GlobalSurfaceWater

## Exported outputs

- Krishna_Budameru_DEM.tif
- Krishna_Budameru_Flood_Extent_2024.tif
- Krishna_Budameru_NDVI_FIXED_2024.tif
- Krishna_Budameru_NDWI_2024.tif
- Krishna_Budameru_NDWI_Water_Mask_2024.tif
- Krishna_Budameru_Slope.tif

## Download Access

The exported Google Earth Engine outputs are available through the following Google Drive folder:

[Download Krishna–Budameru GEE Outputs](https://drive.google.com/drive/folders/1bstTY9w1kXmEMgRQRfkhcHZdKo_4xJ6g?usp=drive_link)

The folder contains exported analysis outputs, including:

- Krishna_Budameru_DEM.tif
- Krishna_Budameru_Flood_Extent_2024.tif
- Krishna_Budameru_NDVI_FIXED_2024.tif
- Krishna_Budameru_NDWI_2024.tif
- Krishna_Budameru_NDWI_Water_Mask_2024.tif
- Krishna_Budameru_Slope.tif

The source satellite data are accessed through Google Earth Engine.  
Exported products are derived analysis outputs, not original satellite scenes.

## Processing record

Record the actual dates, orbit filters, thresholds, cloud masking,
export resolution, and coordinate reference system used in each script.
## Outputs

The exported Google Earth Engine outputs are available here:

[Download GEE Outputs](https://drive.google.com/drive/folders/1bstTY9w1kXmEMgRQRfkhcHZdKo_4xJ6g?usp=drive_link)

| Item                   | GitHub lo pettala? | Drive lo pettala? |
| ---------------------- | ------------------ | ----------------- |
| Main flood map         | Yes                | Yes               |
| NDVI map               | Yes                | Yes               |
| NDWI map               | Yes                | Yes               |
| Elevation map          | Yes                | Yes               |
| Slope map              | Yes                | Yes               |
| Final flood-prone map  | Yes                | Yes               |
| Large GeoTIFF files    | No                 | Yes               |
| Full documentation PDF | Yes                | Yes               |
| Raw exported outputs   | Optional           | Yes               |
