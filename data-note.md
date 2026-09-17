Week 2 Data Note

1. Watercourses / Drainage Network
Source: OpenStreetMap via Geofabrik / QuickOSM Plugin (https://download.geofabrik.de/africa/nigeria.html)
Geometry Type: Line(LineString)
Feature Count: 142 features
Key Columns:`fid`, `full_id`, `osm_id`, `osm_type`, `waterway`
Data Quality Notes: Core spatial attributes (`osm_id`, `waterway`) are completely filled for all line features. Secondary attributes like `GNS:id` contain missing (`NULL`) values.

2. Digital Elevation Model (DEM) / Slope
Source: OpenTopography — SRTM GL1 30m Global DEM (https://portal.opentopography.org/datasets)
Geometry Type: Raster (30m spatial resolution)
Feature Count: Single-band elevation raster grid
Key Columns / Attributes: Band 1 Pixel Values (Elevation in meters above sea level)
Data Quality Notes: Seamless digital surface model with zero `NoData` void holes across the entire Ibadan North boundary. Ready for slope gradient extraction.

3. Administrative Boundaries (Ibadan North LGA)
Source: GRID3 Nigeria Open Data Hub (https://data.grid3.org)
Geometry Type: Polygon (Vector)
Feature Count: 12 ward polygons
Key Columns: `ward_id`, `ward_name`, `lga_name`, `state_name`
Data Quality Notes: High-precision administrative vector boundaries with 100% attribute field completeness and no self-intersecting polygon errors.

4. Precipitation / Rainfall Data
Source: Climate Engine — CHIRPS Monthly Precipitation (https://app.climateengine.org/climateEngine)
Geometry Type: Raster (~5km spatial resolution)
Feature Count: Single-band monthly rainfall grid
Key Columns / Attributes: Band 1 Pixel Values (Precipitation in mm)
Data Quality Notes: Coarse resolution compared to DEM, but provides complete spatial coverage across the study area for interpolation.

5. Geology / Lithology Map
Source: Digital Geological Map of Nigeria via Zenodo Repository (https://zenodo.org/records/17216526)
Geometry Type: Polygon / GeoTIFF Raster
Feature Count: Regional geological unit polygons
Key Columns: `litho_unit`, `rock_type`, `formation`
Data Quality Notes: Regional-scale lithological units require georeferencing and clipping to the Ibadan North LGA boundary.
