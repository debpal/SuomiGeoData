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


Download by Labels
--------------------
Download topographic database shapefiles using label names.

.. code-block:: python
    
    # download topographic database using labels
    paituli.tdb_download_by_labels(
        labels=['K2344R', 'J3224R'], 
        folder_path=r"C:\Users\Username\Folder"
    )
    
    
Metadata 
-----------
Convert the topographic database metadata into a readable MultiIndex DataFrame.

.. code-block:: python

    paituli.tdb_metadata_to_dataframe(
        excel_file=r"C:\Users\Username\Folder\tdb_metadata.xlsx"
    )





    
