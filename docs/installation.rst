==============
Installation
==============

The installation of the package is straightforward. To prevent conflicts with other Python packages, it is recommended to create a separate Python environment. 
Below are the steps for installing the package using different methods.


Create a Python environment
-----------------------------

Suppose your environment name is my_env, and you can create it by using the following steps through Anaconda distribution.

.. code-block:: console
    
    conda create --name my_env
    conda activate my_env
    conda install pip


Install from PyPI
-------------------

.. code-block:: console
    
    pip install SuomiGeoData



Install from GitHub repository
--------------------------------

.. code-block:: console

    pip install git+https://github.com/debpal/SuomiGeoData.git
    
    
Install from source code in editable mode
--------------------------------------------

For developers who want to modify the source code or contribute to the package, it is recommended to install in editable mode.
Navigate to your directory with the `my_env` Python environemnt activated, and run the following commands. 
This allows you to make changes to the source code, with immediate reflection in the `my_env` environment without requiring reinstallation.

.. code-block:: console

    pip install build
    git clone https://github.com/debpal/SuomiGeoData.git
    cd SuomiGeoData
    python -m build
    pip install -e .
