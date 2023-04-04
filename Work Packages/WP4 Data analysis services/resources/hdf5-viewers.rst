====================
 HDF5/NeXus viewers
====================

This document provides a list of links to open source `HDF5 <https://www.hdfgroup.org/solutions/hdf5/>`_/NeXus_ data file format viewers and to lists maintained on other websites.
Please add links to any missing relevant application.

In jupyter lab/notebooks
========================

- `h5glance <https://pypi.org/project/h5glance/>`_ lets you explore HDF5 files in the terminal or an HTML interface.
- `jupyterlab-h5web <https://pypi.org/project/jupyterlab-h5web/>`_ is a JupyterLab extension to explore and visualize HDF5 file contents, using the web-based viewer h5web_. h5web supports the NeXus_.
- `hdfviewer <https://pypi.org/project/hdfviewer/>`_ is a python3 package for inspecting HDF files in the context of Jupyter Lab notebook.

Web-based
=========

- `myHDF5.hdfgroup.org <https://myhdf5.hdfgroup.org/>`_: Online HDF5 file viewing service. It is based on `H5Web <https://github.com/silx-kit/h5web/>`_, a React/WebGL viewer for exploring and visualising HDF5 files, as well as h5wasm_, a WebAssembly port of the HDF5 C library that allows reading HDF5 files with JavaScript.
- h5web_ (`online demo <https://h5web.panosc.eu/>`_): A collection of React components to visualize and explore data including **@h5web/app** a component to explore and visualize data stored in HDF5 (or HDF5-like) files, and data providers to connect this component to various back-end solutions.
- `hdf5-web-gui <https://gitlab.com/MAXIV-SCISW/HDF5-VIEWER/hdf5-web-gui>`_ (`online demo <http://demo.maxiv.lu.se/hdf5-web-gui/html/>`_):
  A web GUI for viewing the contents of HDF5 files, using hdf5-simple-server in the backend.
- `h5nuvola <https://github.com/ElettraSciComp/h5nuvola>`_: Web interface and services for remote data browsing and visualisation of HDF5 files.
- `hsds-viz <https://github.com/NREL/hsds-viz>`_: Web viewer developed by NREL for the WIND dataset. Based on `HSDS <https://github.com/HDFGroup/hsds>`_.

Desktop
=======

* From the `HDFGroup <https://www.hdfgroup.org/>`_:

  - `HDFView <https://www.hdfgroup.org/downloads/hdfview/>`_ is a visual tool written in Java for browsing and editing HDF (HDF5 and HDF4) files.
  - `HDF Compass <https://github.com/HDFGroup/hdf-compass>`_ is an experimental viewer program for HDF5 and related formats, designed to complement other more complex applications like HDFView.

* `List of data analysis tools <http://download.nexusformat.org/doc/html/utilities.html#data-analysis>`_ with NeXus_ support from the NeXus_ website.

* Other Python-based viewers not mentioned in previous lists:

  - `ViTables <http://vitables.org/>`_ is a GUI for browsing and editing files in both PyTables and HDF5 formats.
  - `h5pyViewer <https://pypi.org/project/h5pyViewer>`_ contains classes and tools to view *.hdf5 files.
  - `silx view <http://www.silx.org/doc/silx/latest/applications/view.html>`_ command is provided to open data files in a graphical user interface.
  - `NexPy <https://github.com/nexpy/nexpy>`_ provides tools to access/write NeXus files in Python and a simple GUI. The linked project `NXremote <https://github.com/nexpy/nxremote>`_ allows for remote access to NeXus files.

* `List of viewers for HDF-EOS (Hierarchical Data Format - Earth Observing System) <http://hdfeos.org/software/tool.php#HDFVIEW>`_

* `Visual Studio Code <https://code.visualstudio.com/>`_ extension:

  - `VSCode-H5Web <https://marketplace.visualstudio.com/items?itemName=h5web.vscode-h5web>`_: Explore and visualise HDF5 files directly in Visual Studio Code with h5web_ and h5wasm_.

.. _h5wasm: https://github.com/usnistgov/h5wasm
.. _h5web: https://github.com/silx-kit/h5web/
.. _NeXus: https://www.nexusformat.org/
