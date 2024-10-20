============
Land Cover
============

A brief overview of the features related to land cover.


Class Instance
----------------
Let's start by instantiating the class.

.. code-block:: python

    import SuomiGeoData
    paituli = SuomiGeoData.Paituli()
    syke = SuomiGeoData.Syke()


Download Land Cover
---------------------
Get the land cover map.

.. code-block:: python

    syke.download_corine_land_cover_2018(
        folder_path=r"C:\Users\Username\Folder"
    )
    
    
Clipped Land Cover 
--------------------
Get the clipped land cover for the example area.

.. code-block:: python

    # save the example area
    example_gdf = paituli.get_example_area
    example_file = r"C:\Users\Username\Folder\example.shp"
    example_gdf.to_file(example_file)
    
    # instantiation of Core class
    core = SuomiGeoData.core.Core()
    
    # clipped land cover for the example area
    core.raster_clipping_by_mask(
        input_file=r"C:\Users\Username\Folder\Clc2018_FI20m.tif",
        mask_file=example_file,
        output_file=r"C:\Users\Username\Folder\example_land_cover.tif"
    )
    
