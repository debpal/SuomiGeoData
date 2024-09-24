===========
Introdution
===========


SuomiGeoData is a Python package whose concept originated on September 11, 2024. It is designed to simplify the process of downloading and extracting geospatial data from Suomi, that is Finland. The package offers the following features:


* `Paituli integration <https://paituli.csc.fi/download.html>`_

    - Provides access to vector format index maps for downloading DEM and the topographic database.
    - Downloads DEM as raster files and the topographic database as shapefiles based on label names from the index maps.
    - Downloads all DEM labels intersected with a given vector format area.
    - Downloads clipped DEM data that matches a given vector format area.
    
* `SYKE integration <https://www.syke.fi/en-US/Open_information/Spatial_datasets/Downloadable_spatial_dataset>`_

    - Downloads CORINE land cover 2018 raster.
    - Downloads vector files of latest subcatchment divisions, ranging from level 1 to 5.
    - Extracts individual or merged subcatchments by identifier and uses these areas to download DEM.
    
* Geoprocessing

    - Simplified merging and clipping of raster files.