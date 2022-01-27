Use Case 28 - Online visualisation, exploration and analysis of HDF5 files with h5nuvola.md
=========================================================
[HDF5](http://www.hdfgroup.org/) is a de-facto standard for storage of heterogeneous, n-dimensional  scientific data. It is portable, without vendor lock-in, self-describing thanks to included metadata, with libraries in different languages. It offers high I/O performance, optimised for both time and storage.

One of the disadvantages of this format is the need for specialised applications to work with data from hdf5 files. HDFGroup itself offers standalone software like HDFView that can be downloaded, while other actors shared tools such as H5Web with the scientific community, to visualise such data.

With this use case we designed and developed h5nuvola, a web tool written in Python, based on the popular Django framework. h5nuvola can be linked to one or more data sources, being local folders, NFSs, etc., and uses metadata and hard logic to select from a set of visualisation plugins, being them general purposed (like the ones for 1 and 2 dimensional datasets) or customised for specific applications (such as one designed to view, explore and analyse X-Ray Fluorescence datasets).

Custom applications are easy to implement, relying on Dash-Plotly applications, written in  pure Python, and making easy the integration of interactive controls, callbacks, and the use of scientists’ analytic pipelines.


Main Contributors
------
* **Andrea Lorenzon** – Software engineering, main developer
* **Georgios Kourousias** – Concept, supervisor, initial development
* **Marco De Simone** – System integration, DevOps
* **Emiliano Coghetto** – Integration with Elettra Virtual Unified Office
* **Alessandro Olivo** – Testing

Use Case Action Flow
------
* **Browing** – Visit h5nuvola home page, and browse file included in your attached data sources
* **Select a file** – Quick search available: typing few letters of the filename will help in finding your data
* **Select a dataset** – Quick search available
* **Automatic redirection to an appropriate app** – h5nuvola will redirect users, dispatching to an appropriate app to explore your data
* **Perform analytics** – Use app’s analytical tools to extract information from data

Description of needs
------
The service will be integrated into the CERIC-ERIC EOSC service portfolio. h5nuvola will progressively fit more in the PaNOSC universe, and as soon as metadata will be included in h5 files and users will create and share more apps.

Furthermore, the Search API and Data Catalog will integrate current data browsing. Eventually, OAUTH2 or other authentication authorities (that are already supported) will be included.

Impacts from the implementation
------
Remote authorised users will be able to visualise and analyse shared hdf5 files datasets without the need to install software. Immediate visual feedback, with interactive plots and online analysis tools, will make their workflow more transparent, reproducible and machine-independent. 

A galaxy of h5nuvola apps can be shared by users, improving collaboration and progress of research.

Generalisation of the use case
Any hdf5 user can benefit from h5nuvola. Any kind of data, even non-PaN, can have a dedicated app.

It is also possible to include backend-powered computation for online processing of datasets, making the data pipeline process potentially transparent to scientists, letting them concentrate on results.

While h5nuvola is not indicated for non-standard analysis pipelines, that could find a better tool in a Jupyter Notebook instance, it makes fast exploration of hdf5 a reality.

Other partners interested in this use case
------
Elettra, and any other partner using hdf5 as a standard data format, could be interested.

Resources
------
* **Web framework**: django
* **HDF5 access**: h5py
* **web app management**: Dash
* **Dash application wrapper for Django**: django-plotly-dash
* **Session management**: redis
* **app database**: postgres
* **Data visualisation**: plotly, ev. matplotlib
* **Data processing**: numpy, scipy, opencv2…
* **[Software and documentation repository](https://gitlab.elettra.eu/panosc/h5nuvola)**

PaNOSC related work packages
------
[WP4 – Data analysis services](https://www.panosc.eu/work-packages/work-package-4-data-analysis-services/)

Contact person
------
[Andrea Lorenzon](mailto:andrea.lorenzon@ceric-eric.eu) (CERIC-ERIC)


