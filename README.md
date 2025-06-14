# SuomiGeoData


| <big>Status</big> | <big>Description</big> |
| --- | --- |
| **PyPI**| ![PyPI - Version](https://img.shields.io/pypi/v/SuomiGeoData) ![PyPI - Status](https://img.shields.io/pypi/status/SuomiGeoData) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SuomiGeoData) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/SuomiGeoData) |
| **GitHub** | ![GitHub commit activity](https://img.shields.io/github/commit-activity/t/debpal/SuomiGeoData) ![GitHub last commit](https://img.shields.io/github/last-commit/debpal/SuomiGeoData) [![flake8](https://github.com/debpal/SuomiGeoData/actions/workflows/linting.yml/badge.svg)](https://github.com/debpal/SuomiGeoData/actions/workflows/linting.yml) [![mypy](https://github.com/debpal/SuomiGeoData/actions/workflows/typing.yml/badge.svg)](https://github.com/debpal/SuomiGeoData/actions/workflows/typing.yml) [![pytest](https://github.com/debpal/SuomiGeoData/actions/workflows/testing.yml/badge.svg)](https://github.com/debpal/SuomiGeoData/actions/workflows/testing.yml) |
| **Codecov** | [![codecov](https://codecov.io/gh/debpal/SuomiGeoData/graph/badge.svg?token=ORFQKXO96C)](https://codecov.io/gh/debpal/SuomiGeoData)  |
| **Read** _the_ **Docs** | ![Read the Docs](https://img.shields.io/readthedocs/SuomiGeoData) |
| **PePy** | ![Pepy Total Downloads](https://img.shields.io/pepy/dt/SuomiGeoData) |
| **License** | ![PyPI - License](https://img.shields.io/pypi/l/SuomiGeoData) |

`SuomiGeoData` is a Python package designed to simplify the process of downloading and analyzing geospatial data from Finland, that is Suomi. Conceptualized on September 11, 2024, and launched on September 14, 2024, this package is tailored for users with limited coding experience but still in need powerful geospatial insights. It streamlines the workflow by handling internal complexities, allowing users to focus on desired outputs rather than intermediate steps. The goal of `SuomiGeoData` is to empower users by providing easy access to open-source geodapatial data, enabling informed decision-making by simplified analysis. Currently, the package offers the following features:


## [Paituli integration](https://paituli.csc.fi/download.html)

- Digital Elevation Model (DEM)

    - Provides access to a vector format index map of DEM raster labels.
    - Downloads DEM raster files based on label names from the index map.
    - Downloads raster files of all DEM labels intersecting with a given vector format area.
    - Downloads a clipped DEM raster file that matches a given vector format area.
    * Downloads clipped DEM raster files by [Syke's](https://www.syke.fi/en-US/Open_information/Spatial_datasets/Downloadable_spatial_dataset) subcatchment identifiers.
        
- Topograhic Database
    - Provides access to a vector format index map of topographic database labels.
    - Downloads topographic database folders of shapefiles based on label names from the index map.
    - Downloads shapefile folders of all topographic database labels intersecting with a given vector format area.
    - Downloads topographic database metadata containing the name and class number of the geometric features.
    - Extracts feature geometries based on class number from the shapefile folders.
    - Downloads feature geometries based on class number located within a given vector format area.
    - Downloads feature geometries based on class number and [Syke's](https://www.syke.fi/en-US/Open_information/Spatial_datasets/Downloadable_spatial_dataset) subcatchment identifiers.


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
```

## Documentation

For detailed information, see the [documentation](https://suomigeodata.readthedocs.io/en/latest/).


## Support

If this project has been helpful and you'd like to contribute to its development, consider sponsoring with a coffee! Support will help maintain, improve, and expand this open-source project, ensuring continued valuable tools for the community.

[![Buy Me a Coffee](https://img.shields.io/badge/☕_Buy_me_a_coffee-FFDD00?style=for-the-badge)](https://www.buymeacoffee.com/debasish_pal)















