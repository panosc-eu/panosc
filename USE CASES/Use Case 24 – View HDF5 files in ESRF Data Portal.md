Use Case 24 – View HDF5 files in ESRF Data Portal
=========================================================
The [ESRF data portal](https://data.esrf.fr/) provides access to all raw data files. It would be useful for ESRF users to be able to browse the Nexus structure and display the data using the h5web viewer. This would help users who are not familiar with HDF5 to browse their data. A second objective is to open an HDF5 data file in Jupyterlab and display it with h5web. This will allow users to manipulate their data directly from the data portal.

Main Contributors
------
* **Alex De Maria** – Data Manager and developer and maintainer of the ESRF data portal 
* **Axel Bocciarelli** – Web frontend developer and maintainer of h5web
* **Loic Huder** – Web frontend and backend developer of h5web, Nexus/HDF5 expert

Use Case Action Flow
------
* **Setup h5grove:** Setup a cloud service for the backend, h5grove, for accessing hdf5 files 
* **Data access:** Solve the user AAI for secure data access and provide an infrastructure for h5grove which scales for multiple users
* **Package h5web:** Provide a package of h5web for integration in the data portal
* **Data portal integration:** Modify the data portal to integrate the h5web viewer

Description of needs
------
A Nexus/HDF5 file viewer which can be integrated in a web application.

Impacts from the implementation
------
Users can browse, view, evaluate and download data from the same application

Generalisation of use case
------
Other sites using the same portal as the ESRF (ICAT backend + ICATplus frontend) will be able to deply the solution immediately. Other sites could adopt a similar approach by reusing the backend and integrating h5web into their data portal e.g. SciCat.

Other partners interested in this use case
------
* [ELI ERIC](https://eli-laser.eu/)
* United Kingdom Infra-Red Telescope – UKIRT
* [Diamond Light Source](https://www.diamond.ac.uk/Home.html)
* [ISIS](https://www.isis.stfc.ac.uk/Pages/home.aspx)

Resources
------
* [H5web](https://github.com/silx-kit/h5web)
* [H5grove](https://github.com/silx-kit/h5grove)
* [Jupyterlab-h5web](https://github.com/silx-kit/jupyterlab-h5web)
* [ICATplus frontend](https://gitlab.esrf.fr/icat/E-DataPortal)
* [ICAT server](https://github.com/icatproject/icat.server)

PaNOSC related work packages
------
* [WP3 – Data catalogue services](https://www.panosc.eu/work-packages/work-package-3-data-catalog-services/): Data portal development
* [WP4 – Data analysis services](https://www.panosc.eu/work-packages/work-package-4-data-analysis-services/): H4web development
* [WP6 – EOSC integration](https://www.panosc.eu/work-packages/work-package-6-eosc-integration/): Infrastructure

Contact person
------
[Andy Götz](mailto:andy.gotz@esrf.fr) (ESRF)
