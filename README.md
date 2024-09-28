# SuomiGeoData

SuomiGeoData is a Python package whose concept originated on September 11, 2024. It is designed to simplify the process of downloading and extracting geospatial data from Suomi, that is Finland. The package offers the following features:


* [Paituli integration](https://paituli.csc.fi/download.html)

    - Provides access to vector format index maps for downloading DEM and the topographic database.
    - Downloads DEM as raster files and the topographic database as shapefiles based on label names from the index maps.
    - Downloads all DEM labels intersected with a given vector format area.
    - Downloads clipped DEM data that matches a given vector format area.
    
 * [Syke integration](https://www.syke.fi/en-US/Open_information/Spatial_datasets/Downloadable_spatial_dataset) 

    - Downloads CORINE land cover 2018 raster.
    - Downloads vector files of latest subcatchment divisions, ranging from level 1 to 5.
    - Extracts individual or merged subcatchments by identifier and uses these areas to download DEM.
    
 * Geoprocessing

    - Simplified merging and clipping of raster files.
    
    
## Roadmap

* Enable downloading the topographic database for a specified area using a shapefile.
* Implement searching and merging of features from the downloaded topographic database.


## Easy Installation

To install, use pip:

```bash
pip install SuomiGeoData
```

## Quickstart
A brief example of how to start:

```python
>>> import SuomiGeoData
>>> paituli = SuomiGeoData.Paituli()

# get the topographic database index map
>>> paituli.indexmap_tdb.head()

     label                                               path	                                         geometry
    -------------------------------------------------------------------------------------------------------------
0	K2344R	mml/maastotietokanta/2022/shp/K2/K23/K2344R.sh...	POLYGON ((104000 6606000, 104000 6618000, 1160...
1	K2334R	mml/maastotietokanta/2022/shp/K2/K23/K2334R.sh...	POLYGON ((104000 6582000, 104000 6594000, 1160...
2	K2343R	mml/maastotietokanta/2022/shp/K2/K23/K2343R.sh...	POLYGON ((104000 6594000, 104000 6606000, 1160...
3	K2443L	mml/maastotietokanta/2022/shp/K2/K24/K2443L.sh...	POLYGON ((92000 6642000, 92000 6654000, 104000...
4	K2443R	mml/maastotietokanta/2022/shp/K2/K24/K2443R.sh...	POLYGON ((104000 6642000, 104000 6654000, 1160...
...
```

## Documentation

For detailed information, see the [documentation](http://suomigeodata.readthedocs.io/).


## Toolkit

| <big>Status</big> | <big>Description</big> |
| --- | --- |
| **PyPI**| ![PyPI - Version](https://img.shields.io/pypi/v/SuomiGeoData) ![PyPI - Status](https://img.shields.io/pypi/status/SuomiGeoData) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SuomiGeoData) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/SuomiGeoData) |
| **GitHub** | ![GitHub last commit](https://img.shields.io/github/last-commit/debpal/SuomiGeoData) [![flake8](https://github.com/debpal/SuomiGeoData/actions/workflows/linting.yml/badge.svg)](https://github.com/debpal/SuomiGeoData/actions/workflows/linting.yml) [![mypy](https://github.com/debpal/SuomiGeoData/actions/workflows/typing.yml/badge.svg)](https://github.com/debpal/SuomiGeoData/actions/workflows/typing.yml) [![pytest](https://github.com/debpal/SuomiGeoData/actions/workflows/testing.yml/badge.svg)](https://github.com/debpal/SuomiGeoData/actions/workflows/testing.yml) ![GitHub repo size](https://img.shields.io/github/repo-size/debpal/SuomiGeoData) |
| **Codecov** | [![codecov](https://codecov.io/gh/debpal/SuomiGeoData/graph/badge.svg?token=ORFQKXO96C)](https://codecov.io/gh/debpal/SuomiGeoData)  |
| **Read** _the_ **Docs** | [![Documentation Status](https://readthedocs.org/projects/suomigeodata/badge/?version=latest)](https://suomigeodata.readthedocs.io/en/latest/?badge=latest) |
| **PePy** | ![Pepy Total Downloads](https://img.shields.io/pepy/dt/SuomiGeoData) |
| **License** | ![PyPI - License](https://img.shields.io/pypi/l/SuomiGeoData) |

