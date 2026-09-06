Project Brief - Groundwater Potential Mapping of Ibadan North LGA, Oyo State, Nigeria

Spatial Question - Which areas of Ibadan North Local Government Area have the highest
groundwater potential, based on geology, slope, drainage proximity, and
rainfall?

Study Area - Ibadan North Local Government Area, Oyo State, Nigeria (headquarters: Agodi;
total area approx. 22 km²).

Datasets Required

	1.	Geology / lithology map. Nigeria Geological Map (https://zenodo.org/records/17216526) 
	2.	Elevation (DEM) — [OpenTopography — SRTM GL1 30m](https://portal.opentopography.org/datasets) 
	3.	Drainage network [Geofabrik — Nigeria OSM extract](https://download.geofabrik.de/africa/nigeria.html) 
	4.	Rainfall (precipitation) [Climate Engine — CHIRPS](https://app.climateengine.org/climateEngine) 
	5.	Administrative boundary (Ibadan North LGA) [IGISMAP — Nigeria LGA Boundary Shapefiles](https://www.igismap.com/download-nigeria-shapefile-free-administrative-boundary-state-city-map/) 

Data Status - All datasets above are confirmed to exist and are downloadable directly online.

Method (planned)
1. Download and prepare all datasets listed above.
2. Filter/clip the national LGA boundary layer to Ibadan North only.
3. Clip the DEM, drainage network, geology, and rainfall layers to the Ibadan North boundary.
4. Derive slope from the DEM.
5. Derive distance-to-drainage layer.
6. Reclassify each layer to a common suitability scale.
7. Combine layers (weighted overlay) in QGIS to produce a groundwater potential map for Ibadan North LGA.