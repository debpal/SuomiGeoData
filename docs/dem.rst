=========================
Digital Elevation Model
=========================

A brief overview of the features for working with Digital Elevation Models (DEM).


Class Instance
----------------
Let's start by instantiating the classes.

.. code-block:: python

    import SuomiGeoData
    paituli = SuomiGeoData.Paituli()
    syke = SuomiGeoData.Syke()
    
    
Download by Labels
--------------------
Download DEM using label names.

.. code-block:: python
    
    # download DEM using labels
    paituli.dem_download_by_labels(
        labels=['K3244G', 'X4344A'], 
        folder_path=r"C:\Users\Username\Folder"
    )
    
    
Example area
--------------
Access the example area and plot it.

.. code-block:: python

    example_area = paituli.get_example_area
    # for JupyterLab user
    example_area.iloc[0].geometry
    

.. image:: _static/example_area.JPG
   :scale: 50 %
   :align: center


Clipped DEM
-------------
Get the clipped DEM for the example area.

.. code-block:: python
    
    paituli.dem_clipped_download_by_area(
        input_area=example_area,
        output_file=r"C:\Users\Username\Folder\example_area.tif"
    )
    
    
DEM Labels
------------
Retrieve the DEM labels for the example area, if required.

.. code-block:: python
    
    paituli.dem_labels_download_by_area(
        input_area=example_area,
        folder_path=r"C:\Users\Username\Empty_folder_with_no_files"
    )
    
    
DEM from Syke's Catchment Divison
-----------------------------------
Download the vector files of catchment divisions and obtain DEM data from the subcatchment identifier.

.. code-block:: python
    
    # download catchment divisions
    syke.download_catchment_divisions_2023(
        folder_path=r"C:\Users\Username\Folder\Cactment_Folder"
    )
    
    # get clipped DEM from the subcatchment identifier
    paituli.dem_clipped_download_by_syke_subcatchment(
        input_file=r"C:\Users\Username\Folder\Cactment_Folder\catchment_division_level_5.shp",
        level=5,
        single_area=15730216003,
        output_file=r"C:\Users\Username\Folder\clipped_dem.tif"
    )
    
    # merge mutiple subcatchments that share boundaries and get the clipped DEM
    msc_gdf = syke.merging_multiple_subcatchments(
        input_file=r"C:\Users\Username\Folder\Cactment_Folder\catchment_division_level_5.shp",
        level=5,
        multiple_area=[15730214505, 15730214514],
        percentage_cutoff=0 # read about this parameter in the documentation 
    )
    paituli.dem_clipped_download_by_area(
        input_area=msc_gdf,
        output_file=r"C:\Users\Username\Folder\merged_clipped_dem.tif"
    )