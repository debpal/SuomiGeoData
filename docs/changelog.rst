===============
Release Notes
===============


Version 1.1.2
---------------

* **Release date:** 11-Feb-2025.

* **Compatibity:** Verified with Python 3.13.

Version 1.1.1
---------------

* **Release date:** 20-Oct-2024.

* **Feature Additions:** 

    * Extracts feature geometries based on class number from the shapefile folders of topographic database labels.
    * Downloads feature geometries based on class number located within a given vector format area.
    * Downloads feature geometries based on class number and Syke's subcatchment identifiers.

* **Documentation:** Added a tutorial on how to use the new features.


Version 1.0.1
---------------

* **Release date:** 09-Oct-2024.

* **Feature Additions:** Downloads topographic database metadata and converts to a readble MultiIndex DataFrame.

* **Development status:** Upgraded from Alpha to Beta.


Version 1.0.0
---------------

* **Release date:** 24-Sep-2024.

* **Feature Additions:** 

    * Downloads all DEM labels intersected with a given vector format area.
    * Downloads clipped DEM data that matches a given vector format area.
    * Downloads CORINE land cover 2018 raster data and vector files of subcatchment divisions SYKE's open-source spatial data.
    * Extracts individual or merged subcatchments by identifier and uses these areas to download DEM.
    * Simplified merging and clipping of raster files.

* **Documentation:** Added a tutorial on how to use the new features.

* **Development status:** Upgraded to Alpha from Pre-Alpha.


Version 0.1.0
---------------

* **Release date:** 17-Sep-2024.

* **Feature Additions:** 

    * Access characteristics of the DEM index map.
    * Download selected labels as raster files from the DEM index map.
    * Download selected labels as shapefile folders from the topographic database index map.

* **GitHub Actions Integration:**

    * Linting with `flake8` to enforce PEP8 code formatting.
    * Type checking with `mypy` to verify annotations throughout the codebase.
    * Code testing with `pytest` to ensure code reliability.
    * Test Coverage with **Codecov** to monitor and report test coverage.
    
* **Compatibity:** Verified with Python 3.10, 3.11, and 3.12.

* **Documentation:** Added new badges to `README.md` to display statuses for linting, type-checking, testing, and coverage.

* **Development status:** Upgraded to Pre-Alpha from Planning.


Version 0.0.1
---------------

* **Release date:** 14-Sep-2024.

* **Features:** Functionality for accessing the characteristics of topographic database index map.

* **Development status:** Planning.

* **Roadmap:** Ongoing addition of new features.