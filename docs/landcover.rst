===========
Land Cover
===========

A brief overview of the features related to land cover.


Class Instance
-----------------
Let's start with the instantiation of the class:

.. code-block:: python

    import SuomiGeoData
    paituli = SuomiGeoData.Paituli()
    syke = SuomiGeoData.Syke()


Download Land Cover
----------------------
Get the land cover map:

.. code-block:: python

    syke.download_corine_land_cover_2018(
        folder_path=r"C:\Users\Username\Land_cover_folder"
    )
    
    
Clipped Land Cover 
--------------------
Get the clipped land cover for the example area:

.. code-block:: python

    # example area
    example_area = paituli.get_example_area
    
    # instantiation of Core class
    core = SuomiGeoData.core.Core()
    
    # clipped land cover for the example area
    core.raster_clipping_by_mask(
        input_file=r"C:\Users\Username\Land_cover_folder\Clc2018_FI20m.tif",
        mask_area=example_area,
        output_file=r"C:\Users\Username\Folder\example_land_cover.tif"
    )
    
    # clipped land cover for the example area with buffer
    example_area['geometry'] = example_area.geometry.buffer(200)
    core.raster_clipping_by_mask(
        input_file=r"C:\Users\Username\Land_cover_folder\Clc2018_FI20m.tif",
        mask_area=example_area,
        output_file=r"C:\Users\Username\Folder\example_land_cover_buffer.tif"
    )





    
