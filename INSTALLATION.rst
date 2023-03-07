============
Installation
============

Fiona has several `extension modules
<https://docs.python.org/3/extending/extending.html>`__ which link against the
GDAL project's libgdal. This complicates installation because libgdal is not
generally included by default with computer operating systems.

Binary distributions
====================

Binary distributions (wheels) containing libgdal and its own dependencies are
available from the Python Package Index and can be installed using `pip`.

.. code-block:: console

    pip install fiona

These wheels are mainly intended to make installation easy for simple
applications, like CI for projects that depend on Fiona, not so much for
production. They are not tested for compatibility with all other binary wheels,
conda packages, or QGIS, and omit many of GDAL's optional format drivers.

Many users find Anaconda and conda-forge a good way to install Fiona.
Fiona's conda-forge packages are generally compatible with other conda-forge
packages and share a dependency on a recent version of libgdal which includes
more format drivers than do the pip packages on PyPI.

.. code-block:: console

   conda install -c conda-forge fiona

Installing 
Fiona 1.9 (coming soon) requires Python 3.7 or higher and GDAL 3.2 or higher.
