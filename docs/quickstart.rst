============
Quickstart
============

This guide provides a quick overview to get started with :mod:`SuomiGeoData`.


Verify Installation
---------------------
Ensure successful installation by running the following commands.

.. code-block:: python

    import SuomiGeoData
    paituli = SuomiGeoData.Paituli()
    
    
Index Map
-----------
Access and save the DEM index map.

.. code-block:: python

    dem_gdf = paituli.indexmap_dem
    dem_gdf.head()
    # save the map with 'True' message a output
    paituli.save_indexmap_dem(
        file_path=r"C:\Users\Username\Folder\indexmap_dem.shp"
    )
    
Expected output:

.. code-block:: text

         label	                                   path	                                         geometry
    0	K3244G	mml/dem2m/2008_latest/K3/K32/K3244G.tif	POLYGON ((206000 6654000, 206000 6660000, 2120...
    1	K3244H	mml/dem2m/2008_latest/K3/K32/K3244H.tif	POLYGON ((206000 6660000, 206000 6666000, 2120...
    2	K3222E	mml/dem2m/2008_latest/K3/K32/K3222E.tif	POLYGON ((128000 6654000, 128000 6660000, 1340...
    3	K3222A	mml/dem2m/2008_latest/K3/K32/K3222A.tif	POLYGON ((116000 6654000, 116000 6660000, 1220...
    4	K3222C	mml/dem2m/2008_latest/K3/K32/K3222C.tif	POLYGON ((122000 6654000, 122000 6660000, 1280...


Labels
--------
Retrieve the list of label names for the topographic database.

.. code-block:: python
    
    tdb_labels = paituli.tdb_labels
    
Expected output:

.. code-block:: text

    ['K2344R',
     'K2334R',
     'K2343R',
     'K2443L',
     'K2443R',
     ...]
