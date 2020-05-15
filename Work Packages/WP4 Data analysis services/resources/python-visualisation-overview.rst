Python Visualisation Overview
=============================

This document aims to summarise the state of the python visualisation
ecosystem, with a focus on interactive plotting inside jupyter notebooks.

The most popular visualisation libraries in python are:

-  Matplotlib - https://github.com/matplotlib/matplotlib
-  ggpy - https://github.com/yhat/ggpy
-  plotnine - https://github.com/has2k1/plotnine
-  Bokeh - https://github.com/bokeh/bokeh
-  Plotly - https://github.com/plotly/plotly.py
-  Pygal - https://github.com/Kozea/pygal
-  Altair - https://github.com/altair-viz/altair
-  Gleam - https://github.com/dgrtwo/gleam
-  mpld3 - https://github.com/mpld3/mpld3
-  VisPy - https://github.com/vispy/vispy
-  pyqtgraph - https://github.com/pyqtgraph/pyqtgraph
-  Chaco - https://github.com/enthought/chaco
-  vtki - https://github.com/vtkiorg/vtki

Some libraries are excluded from this list (e.g.
`Seaborn <https://github.com/mwaskom/seaborn>`__,
`Gleam <https://github.com/dgrtwo/gleam>`__,
`mpld3 <https://github.com/mpld3/mpld3>`__,
`HoloViews <https://github.com/pyviz/holoviews>`__) because they build   
on top of existing libraries, as such they inherit many of the problems  
and the (lack of) speed of their parent.

Interesting links:

-  https://towardsdatascience.com/reviewing-python-visualization-packages-fa7fe12e622b
-  https://www.anaconda.com/python-data-visualization-2018-why-so-many-libraries
-  https://pbpython.com/altair-intro.html
-  https://pbpython.com/effective-matplotlib.html
-  https://labs.spotify.com/2018/11/15/introducing-chartify-easier-chart-creation-in-python-for-data-scientists/
-  https://www.youtube.com/watch?v=FytuB8nFHPQ
-  https://pbpython.com/visualization-tools-1.html

Matplotlib
----------

https://github.com/matplotlib/matplotlib

https://matplotlib.org/users/index.html

https://matplotlib.org/

    Matplotlib is a Python 2D plotting library which produces
    publication-quality figures in a variety of hardcopy formats and     
    interactive environments across platforms. Matplotlib can be used in 
    Python scripts, the Python and IPython shell (à la MATLAB or
    Mathematica), web application servers, and various graphical user    
    interface toolkits.

ggpy
----

https://github.com/yhat/ggpy

https://yhat.github.io/ggpy

    ggplot is a Python implementation of the grammar of graphics. It is  
    not intended to be a feature-for-feature port of ggplot2 for
    R--though there is much greatness in ggplot2, the Python world could 
    stand to benefit from it.

Bokeh
-----

https://github.com/bokeh/bokeh

https://bokeh.pydata.org/en/latest/docs/user\_guide.html

http://bokeh.pydata.org/en/latest/

    Bokeh is an interactive visualization library for Python that      
    enables beautiful and meaningful visual presentation of data in    
    modern web browsers. With Bokeh, you can quickly and easily create 
    interactive plots, dashboards, and data applications.

    Bokeh provides an elegant and concise way to construct versatile   
    graphics while delivering high-performance interactivity for large 
    or streamed datasets.

Plotly
------

https://github.com/plotly/plotly.py

https://plot.ly/python/

https://plot.ly/

    plotly.py is an interactive, open-source, and browser-based graphing 
    library for Python sparkles

    Built on top of plotly.js, plotly.py is a high-level, declarative
    charting library. plotly.js ships with over 30 chart types,
    including scientific charts, 3D graphs, statistical charts, SVG
    maps, financial charts, and more.

Pygal
-----
 
https://github.com/Kozea/pygal

http://www.pygal.org/en/stable/

    pygal is a dynamic SVG charting library written in python.

Altair
------

https://github.com/altair-viz/altair

https://altair-viz.github.io/

    Altair is a declarative statistical visualization library for
    Python. With Altair, you can spend more time understanding your data
    and its meaning. Altair's API is simple, friendly and consistent and
    built on top of the powerful Vega-Lite JSON specification. This
    elegant simplicity produces beautiful and effective visualizations
    with a minimal amount of code. Altair is developed by Jake
    Vanderplas and Brian Granger in close collaboration with the UW
    Interactive Data Lab.

VisPy
-----

https://github.com/vispy/vispy

http://vispy.org/documentation.html

http://vispy.org/

    VisPy is a high-performance interactive 2D/3D data visualization
    library. VisPy leverages the computational power of modern Graphics
    Processing Units (GPUs) through the OpenGL library to display very
    large datasets. Applications of VisPy include:

    -  High-quality interactive scientific plots with millions of
       points.
    -  Direct visualization of real-time data.
    -  Fast interactive visualization of 3D models (meshes, volume
       rendering).
    -  OpenGL visualization demos.
    -  Scientific GUIs with fast, scalable visualization widgets (Qt or
       IPython notebook with WebGL).

PyQtGraph
---------

https://github.com/pyqtgraph/pyqtgraph

http://www.pyqtgraph.org/documentation/

http://www.pyqtgraph.org/

    PyQtGraph is intended for use in mathematics / scientific /
    engineering applications. Despite being written entirely in python,
    the library is fast due to its heavy leverage of numpy for number
    crunching, Qt's GraphicsView framework for 2D display, and OpenGL
    for 3D display.

Chaco
-----

https://github.com/enthought/chaco

http://docs.enthought.com/chaco/user\_manual/index.html

http://docs.enthought.com/chaco/

    Chaco is a Python plotting application toolkit that facilitates
    writing plotting applications at all levels of complexity, from
    simple scripts with hard-coded data to large plotting programs with
    complex data interrelationships and a multitude of interactive
    tools. While Chaco generates attractive static plots for publication
    and presentation, it also works well for interactive data
    visualization and exploration.

vtki
----

https://github.com/vtkiorg/vtki

http://docs.vtki.org/

    vtki is a helper module for the Visualization Toolkit (VTK) that
    takes a different approach on interfacing with VTK through NumPy and
    direct array access. This package provides a Pythonic,
    well-documented interface exposing VTK's powerful visualization
    backend to facilitate rapid prototyping, analysis, and visual
    integration of spatially referenced datasets.
