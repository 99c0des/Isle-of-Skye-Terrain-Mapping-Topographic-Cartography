# Isle of Skye | Terrain Mapping & Topographic Cartography

A GIS-based topographic mapping project exploring the terrain, elevation and physical geography of Scotland's Isle of Skye using Digital Elevation Model (DEM) processing, terrain visualisation and cartographic design.

<p align="center">
  <img
    src="Map/isle of skye v2.png"
    alt="Isle of Skye – Topographic Mapping and Terrain Visualisation"
    width="100%"
  >
  <br>
  <em>Topographic visualisation of the Isle of Skye, Scotland.</em>
</p>


## Project Overview

This project focuses on creating a detailed topographic representation of the Isle of Skye, located in the Inner Hebrides of Scotland.

Using Copernicus DEM GLO-30 elevation data, QGIS and GDAL, the project explores terrain characteristics through elevation visualisation, hillshade modelling and contour extraction.

The final objective is to produce a visually informative and geographically meaningful topographic map that communicates the island's distinctive mountainous landscape, elevation variations and coastal geography.

## Study Area

**Location:** Isle of Skye, Inner Hebrides, Scotland, United Kingdom.

The Isle of Skye is characterised by rugged mountain ranges, volcanic landforms, dramatic coastlines, elevated plateaus and deeply dissected valleys.

Its varied terrain makes it an interesting study area for digital elevation modelling and topographic cartography.

## Objectives

- Acquire and process high-resolution elevation data.
- Extract the Isle of Skye study area from larger geographic datasets.
- Generate a terrain hillshade using GDAL.
- Produce 20-metre and 100-metre elevation contours.
- Visualise elevation differences through hypsometric tinting.
- Integrate multiple terrain datasets into a coherent cartographic composition.
- Produce a publication-quality topographic map.

## Data Sources

| Dataset | Source | Purpose |
|---|---|---|
| Copernicus DEM GLO-30 | OpenTopography | Elevation modelling |
| OpenStreetMap | Geofabrik | Island boundary extraction and geographic reference data |

## Software and Tools

- **QGIS:** GIS processing, spatial data management and cartographic design.
- **GDAL:** Raster processing and hillshade generation.
- **OpenTopography:** Elevation data acquisition.
- **OpenStreetMap:** Geographic reference data.

## Methodology

### 1. Data Acquisition
Obtained Copernicus DEM GLO-30 elevation data through OpenTopography and geographic boundary data from OpenStreetMap.

### 2. Study Area Extraction
Identified the Isle of Skye within the source geographic dataset and extracted its boundary for use as the study area.

### 3. DEM Processing
Reprojected the elevation raster to WGS 84 / Pseudo-Mercator (EPSG:3857) and clipped it to the Isle of Skye boundary.

### 4. Hillshade Generation
Generated a hillshade raster independently using GDAL to represent terrain illumination and enhance the visual interpretation of mountain ridges, valleys and slopes.

### 5. Contour Generation
Generated two contour datasets from the processed elevation raster:

- Minor contours: 20-metre intervals.
- Major contours: 100-metre intervals.

### 6. Hypsometric Tinting
Applied a graduated colour scheme to represent elevation differences across the island, using muted earthy and highland-inspired tones.

### 7. Cartographic Design
Integrated the elevation raster, hillshade and contour layers in QGIS. Applied custom symbology, transparency, typography and layout elements to produce the final topographic composition.

## Cartographic Design

The map uses a muted colour palette inspired by traditional topographic and geographical atlases.

| Map Element | Colour |
|---|---|
| Background / Water | `#C9D9D9` |
| Lower Elevation | `#D9C5A3` |
| Low Hills | `#B7B18A` |
| Mid Elevation | `#8F9C78` |
| High Elevation | `#788B78` |
| Highest Terrain | `#687B72` |
| Minor Contours | `#D9C2A3` |
| Major Contours | `#49372D` |
| Labels | `#392F29` |

## Outputs

The project produces the following GIS and cartographic outputs:

- Clipped and reprojected elevation raster.
- Terrain hillshade raster.
- 20-metre contour dataset.
- 100-metre contour dataset.
- Hypsometric elevation visualisation.
- Final topographic map layout.

## Coordinate Reference System

**WGS 84 / Pseudo-Mercator (EPSG:3857)**

The project uses EPSG:3857 for map visualisation and cartographic presentation.

Note that Web Mercator introduces spatial distortion, particularly in distance and area measurements. It is therefore not recommended for precise terrain measurements or area-based analysis.

## Limitations

- The elevation model has a nominal source resolution of approximately 30 metres.
- Reprojection to EPSG:3857 changes the raster's output pixel dimensions and does not increase its original spatial detail.
- Hillshade is a visual terrain representation and does not independently describe slope stability or other physical terrain properties.
- Contour accuracy depends on the quality and resolution of the underlying elevation data.
- The project focuses on terrain visualisation and cartographic representation rather than detailed geomorphological analysis.

## Credits and Acknowledgements

**Elevation Data:** Copernicus DEM GLO-30, accessed through OpenTopography.

Copernicus DEM data attribution: © DLR e.V. 2010–2014 and © Airbus Defence and Space GmbH 2014–2018, provided under COPERNICUS by the European Union and ESA.

**Geographic Data:** © OpenStreetMap contributors, available under the Open Database License (ODbL).

**GIS Processing:** QGIS and GDAL.

## Author

**Gunjan Gautam**

GIS | Remote Sensing | Environmental Mapping | Spatial Analysis

---

This project was developed as part of my GIS portfolio/ passion project focused on geospatial analysis, terrain modelling and cartographic visualisation.<img width="4960" height="3507" alt="isle of skye v2" src="https://github.com/user-attachments/assets/53201894-8119-4a70-9e16-2b832c9ed765" />
