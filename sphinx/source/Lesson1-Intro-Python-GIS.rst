Introduction to Python GIS
==========================

General overview of the latter part of the course
-------------------------------------------------

Now as we know `the basics of Python programming <https://geo-python.github.io>`_ we are ready to
apply those skills to different GIS related tasks. During the next
seven weeks we will learn how to deal with spatial data and analyze it
using "pure" Python.

Learning objectives
-------------------

At the end of the course you should be able to:

-  Read / write spatial data from/to different file formats
-  Deal with different projections
-  Do different geometric operations and geocoding
-  Reclassify your data based on different criteria
-  Do spatial queries
-  Do simple spatial analyses
-  Visualize data and create (interactive) maps, such as following:

.. raw:: html
   :file: bokeh_html/precip_sw_2018-03-02.html


.. raw:: html
  :file: bokeh_html/sw_catch_2018-03-02.html

Why Python for GIS?
-------------------

Python is extremely useful language to learn in terms of GIS since many
(or most) of the different GIS Software packages (such as ArcGIS, QGIS,
PostGIS etc.) provide an interface to do analysis using Python
scripting. During this course, we will mostly focus on doing GIS without
any third party softwares such as ArcGIS. **Why?** There are several
reasons for doing GIS using Python without any additional software:

-  **Everything is free**: you don't need to buy and expensive license
   for ArcGIS (for example)
-  You will **learn and understand** much more deeply how different
   geoprocessing operations work
-  Python is **highly efficient**: used for analysing Big Data
-  Python is **highly flexible**: supports all data formats that you can
   imagine
-  Using Python (or any other open-source programming language)
   **supports open source softwares/codes and open science** by making
   it possible for everyone to reproduce your work, free-of-charge.
-  **Plug-in and chain different third-party softwares** to build e.g. a
   fancy web-GIS applications as you want (using e.g.
   `GeoDjango <https://docs.djangoproject.com/en/1.8/ref/contrib/gis/>`__
   with `PostGIS <http://postgis.net/>`__ as a back-end)

What sort of tools are available for doing GIS in pure Python?
--------------------------------------------------------------

We have already used few Python modules for conducting different tasks,
such as **numpy** for doing mathematical calculations or **matplotlib**
for visualizing our data. From now on, we will familiarize ourselves
with punch of other Python modules that are useful when doing data
analysis or different GIS tasks.

One drawback when compared to using a specific GIS-software such as
`ArcGIS <http://arcgis.com/>`_, is that GIS tools are spread under different Python modules and
created by different developers. This means that you need to familiarize
yourself with many different modules (and their documentation), whereas
e.g. in ArcGIS everything is packaged under a same module called
`arcpy <http://desktop.arcgis.com/en/arcmap/10.3/analyze/arcpy/what-is-arcpy-.htm>`__.

Below we have listed most of the crucial modules (and links to their
docs) that helps you get going when doing data analysis or GIS in
Python. If you are interested or when you start using these modules in
your own work, you should read the documentation from the web pages of
the module that you need:

-  **Data analysis & visualization:**

   -  `Numpy <http://www.numpy.org/>`__ --> Fundamental package for
      scientific computing with Python
   -  `Pandas <http://pandas.pydata.org/>`__ --> High-performance,
      easy-to-use data structures and data analysis tools
   -  `Scipy <http://www.scipy.org/about.html>`__ --> A collection of
      numerical algorithms and domain-specific toolboxes, including
      signal processing, optimization and statistics
   -  `Matplotlib <http://matplotlib.org/>`__ --> Basic plotting library
      for Python
   -  `Bokeh <http://bokeh.pydata.org/en/latest/>`__ --> Interactive
      visualizations for the web (also maps)
   -  `Plotly <https://plot.ly/python/>`__ --> Interactive
      visualizations (also maps) for the web (commercial - free for
      educational purposes)

-  **GIS:**

   -  `GDAL <http://www.gdal.org/>`__ --> Fundamental package for
      processing vector and raster data formats (many modules below
      depend on this). Used for raster processing.
   -  `Geopandas <http://geopandas.org/#description>`__ --> Working with
      geospatial data in Python made easier, combines the capabilities
      of pandas and shapely.
   -  `Shapely <http://toblerity.org/shapely/manual.html>`__ --> Python
      package for manipulation and analysis of planar geometric objects
      (based on widely deployed
      `GEOS <https://trac.osgeo.org/geos/>`__).
   -  `Fiona <https://pypi.python.org/pypi/Fiona>`__ --> Reading and
      writing spatial data (alternative for geopandas).
   -  `Pyproj <https://pypi.python.org/pypi/pyproj?>`__ --> Performs
      cartographic transformations and geodetic computations (based on
      `PROJ.4 <http://trac.osgeo.org/proj>`__).
   -  `Pysal <https://pysal.readthedocs.org/en/latest/>`__ --> Library
      of spatial analysis functions written in Python.
   -  `Geopy <http://geopy.readthedocs.io/en/latest/>`__ --> Geocoding
      library: coordinates to address <-> address to coordinates.
   -  `GeoViews <http://geo.holoviews.org/index.html>`__ --> Interactive
      Maps for the web.
   -  `Networkx <https://networkx.github.io/documentation/networkx-1.10/overview.html>`__
      --> Network analysis and routing in Python (e.g. Dijkstra and A\*
      -algorithms), see `this
      post <http://gis.stackexchange.com/questions/65056/is-it-possible-to-route-shapefiles-using-python-and-without-arcgis-qgis-or-pgr>`__.
   -  `Cartopy <http://scitools.org.uk/cartopy/docs/latest/index.html>`__
      --> Make drawing maps for data analysis and visualisation as easy
      as possible.
   -  `Scipy.spatial <http://docs.scipy.org/doc/scipy/reference/spatial.html>`__
      --> Spatial algorithms and data structures.
   -  `Rtree <http://toblerity.org/rtree/>`__ --> Spatial indexing for
      Python for quick spatial lookups.
   -  `Rasterio <https://github.com/mapbox/rasterio>`__ --> Clean and
      fast and geospatial raster I/O for Python.
   -  `RSGISLib <http://www.rsgislib.org/index.html#python-documentation>`__
      --> Remote Sensing and GIS Software Library for Python.

.. admonition:: Install to your own computer!

    See **directions how to install these modules to your own computer from** `here <Installing_Anacondas_GIS.html>`_
