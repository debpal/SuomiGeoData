# SuomiGeoData

## What is SuomiGeoData?
SuomiGeoData is a Python package designed to simplify the process of downloading and extracting geospatial data from Suomi, that is Finland. The features of the package include:

- **[Paituli](https://paituli.csc.fi/download.html)** 
  - Accessing the topographic database index map.


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
>>> im_tb = paituli.indexmap_tdb
>>> im_tb.shape
(3132, 3)
```

## Documentation

For detailed information, see the [documentation](http://suomigeodata.readthedocs.io/).


## Toolkit

| <big>Status</big> | <big>Description</big> |
| --- | --- |
| **PyPI**| ![PyPI - Version](https://img.shields.io/pypi/v/SuomiGeoData) ![PyPI - Status](https://img.shields.io/pypi/status/SuomiGeoData) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/SuomiGeoData) |
| **GitHub** | ![GitHub last commit](https://img.shields.io/github/last-commit/debpal/SuomiGeoData) [![flake8](https://github.com/debpal/SuomiGeoData/actions/workflows/linting.yml/badge.svg?branch=main)](https://github.com/debpal/SuomiGeoData/actions/workflows/linting.yml) ![GitHub repo size](https://img.shields.io/github/repo-size/debpal/SuomiGeoData) |
| **Codecov** |  |
| **Read**_the_**Docs** | [![Documentation Status](https://readthedocs.org/projects/suomigeodata/badge/?version=latest)](https://suomigeodata.readthedocs.io/en/latest/?badge=latest) |
| **License** | ![PyPI - License](https://img.shields.io/pypi/l/SuomiGeoData) |

