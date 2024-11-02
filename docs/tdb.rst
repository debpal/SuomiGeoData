======================
Topographic Database
======================

A brief overview of the features related to topographic database.


Class Instance
----------------
Let's start by instantiating the class.

.. code-block:: python

    import SuomiGeoData
    paituli = SuomiGeoData.Paituli()
    syke = SuomiGeoData.Syke()


Download by Labels
--------------------
Download topographic database shapefiles using label names.

.. code-block:: python
    
    # download topographic database folders using labels
    paituli.tdb_download_by_labels(
        labels=['K2344R', 'J3224R'], 
        folder_path=r"C:\Users\Username\Folder"
    )
    
    
Metadata of Feature Class
---------------------------
Convert the topographic database metadata into a readable MultiIndex DataFrame 
for a better understanding of the names and class numbers of geometric features.

.. code-block:: python

    paituli.get_tdb_metadata(
        excel_file=r"C:\Users\Username\Folder\tdb_metadata.xlsx"
    )
    

Peatland Drainage Lines by Class Number 
------------------------------------------
Get the peatland drainage lines within the example area.

.. code-block:: python

    # save the example area
    example_gdf = paituli.get_example_area
    example_file = r"C:\Users\Username\Folder\example.shp"
    example_gdf.to_file(example_file)
    
    # peatland drainage lines for class number 36311
    paituli.tdb_feature_extraction_by_area(
        input_file=example_file,
        class_number=36311,
        output_file=r"C:\Users\Username\Folder\example_peatland_drainage.shp"
    )
    
    
Peatland Drainage Lines by Syke's Subcatchment Identifiers 
-------------------------------------------------------------
Retrieve the peatland drainage lines within the specified subcatchment areas, as identified by Syke’s unique subcatchment identifiers.

.. code-block:: python
    
    # download catchment divisions
    syke.download_catchment_divisions_2023(
        folder_path=r"C:\Users\Username\Folderr"
    )
    
    # peatland drainage lines from the subcatchment identifier
    paituli.tdb_feature_extraction_by_syke_subcatchment(
        input_file=r"C:\Users\Username\Folder\catchment_division_level_5.shp",
        level=5,
        id_subcatchments=[15730216003],
        output_file=r"C:\Users\Username\Folder\syke_subcatchment_peatland_drainage.shp"
    )
   
