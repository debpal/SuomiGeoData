=============
Introduction
=============


SuomiGeoData is a Python package designed to simplify the process of downloading and analyzing geospatial data from Finland, that is Suomi. Conceptualized on September 11, 2024, and launched on September 14, 2024, this package is tailored for users with limited coding experience but still in need powerful geospatial insights. It streamlines the workflow by handling internal complexities, allowing users to focus on desired outputs rather than intermediate steps. Active development is ongoing, with exciting new features planned for future releases. The goal of SuomiGeoData is to empower users by providing easy access to open-source geodapatial data, enabling informed decision-making by simplified analysis. Currently, the package offers the following features:


`Paituli integration <https://paituli.csc.fi/download.html>`_
----------------------------------------------------------------

Digital Elevation Model (DEM)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Provides access to a vector format index map of DEM raster labels.
* Downloads DEM raster files based on label names from the index map.
* Downloads raster files of all DEM labels intersecting with a given vector format area.
* Downloads a clipped DEM raster file that matches a given vector format area.
        
Topograhic Database
^^^^^^^^^^^^^^^^^^^^^^
    
* Provides access to a vector format index map of topographic database labels.
* Downloads topographic database folders of shapefiles based on label names from the index map.
* Downloads shapefile folders of all topographic database labels intersecting with a given vector format area.
* Downloads topographic database metadata containing the name and class number of the geometric features.
* Extracts feature geometries based on class number from the shapefile folders.
* Downloads feature geometries based on class number located within a given vector format area.
    
`SYKE integration <https://www.syke.fi/en-US/Open_information/Spatial_datasets/Downloadable_spatial_dataset>`_
-----------------------------------------------------------------------------------------------------------------

* Downloads CORINE land cover 2018 raster.
* Downloads vector files of the latest subcatchment divisions, ranging from level 1 to 5.
* Extracts individual or merged subcatchments by identifier number from the vector files.
* Downloads clipped DEM raster files by subcatchment identifiers.
* Downloads feature geometries based on class number and subcatchment identifiers.
    
