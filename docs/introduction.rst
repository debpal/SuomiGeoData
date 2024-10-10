=============
Introduction
=============


SuomiGeoData is a Python package designed to simplify the process of downloading and analyzing geospatial data from Finland, that is Suomi. Conceptualized on September 11, 2024, and launched on September 14, 2024, this package is tailored for users with limited coding experience but still in need powerful geospatial insights. It streamlines the workflow by handling internal complexities, allowing users to focus on desired outputs rather than intermediate steps. Active development is ongoing, with exciting new features planned for future releases. The goal of SuomiGeoData is to empower users by providing easy access to open-source geodapatial data, enabling informed decision-making by simplified analysis. Currently, the package offers the following features:


* `Paituli integration <https://paituli.csc.fi/download.html>`_

    - Provides access to vector format index maps for downloading DEM and the topographic database.
    - Downloads DEM as raster files and the topographic database as shapefiles based on label names from the index maps.
    - Downloads all DEM labels intersected with a given vector format area.
    - Downloads clipped DEM data that matches a given vector format area.
    - Downloads topographic database metadata and converts to a readble MultiIndex DataFrame.
    
* `SYKE integration <https://www.syke.fi/en-US/Open_information/Spatial_datasets/Downloadable_spatial_dataset>`_

    - Downloads CORINE land cover 2018 raster.
    - Downloads vector files of latest subcatchment divisions, ranging from level 1 to 5.
    - Extracts individual or merged subcatchments by identifier and uses these areas to download DEM.
    
* Geoprocessing

    - Simplified merging and clipping of raster files.