USE CASE HUMAN ORGANS GitHub

Use Case 22 – Human Organs Open Data portal
=========================================================
To make data from the Human Organs Project available as open data via a data portal which supports searching according to the keywords and metadata of the data, e.g. organ, patient, pathology, the data must be referenced by a DOI, archived and downloadable from the ESRF using the ICAT data repository. The portal frontend should be based on the PaNOSC search portal and API.

The project will start with 6 organs and roughly 10 TBs of compressed data. It will continue to grow over the time to eventually contain multi resolution reconstructed volumes of all organs of the human body. The data represent the highest resolution 3D volumes of humans to date.

Main Contributors
------
* **Paul Tafforeau** – Principal Investigator and scientist collecting the data
* **Axel Bocciarelli** – Web developer working on portal frontend
* **Alex de Maria** – Data manager working on ingesting the data and creating the DOIs
* **Marjolaine Bodin** – Data manager working on ingesting the data and creating the DOIs
* **Jiri Majer** - Web developer working on PaN portal

Use Case Action Flow
------
* Curate data: Prepare processed data for ingestion, collect metadata
* Ingest data: Ingest data to ESRF ICAT repository with metadata
* Create DOIs: Create DOIs for the datasets at different levels
* Develop portal: Collect requirements and develop data portal to search and display results
* Link to download: Link the data via the portal to the download service
* Test with users: Test if the portal works as required by typical users

Description of needs
------
Open Data repository, search API, web interface for data portal, display of metadata, download service.

Impacts from the implementation
------
Provide Open Data from the Human Organs Project to the medical research user community for cutting end research in medicine.

Generalisation of use case
------
The dedicated data portal’s frontend could serve for providing data for other scientific communities and domains. The portal could serve as the basis for a generic Open Data portal for searching and downloading data from PaN sites.

Partners
------
All partners with Open Data for a specific community

Resources
------
* ICAT, ICAT+, PaNOSC search API, data portal frontend
* **"Multiscale three-dimensional imaging of intact human organs down to the cellular scale using hierarchical phase-contrast tomography”** Walsh, C.L., Tafforeau, P., Wagner, W.L., Jafree, D.J., Bellier, A., Werlein, C., Kühnel ,M.P., Boller, E., Walker-Samuel, S., Robertus, J-L., Long, D.A., Jacob, J., Marussi, S., Brown, E., Holroyd, N., Jonigk, D.D., Ackermann, M., Lee, P.D., Nat Methods (2021) Accepted

* [Hierarchical Phase-Contrast Tomography (HiP-CT)](https://mecheng.ucl.ac.uk/hip-ct/)

* [Human Organ Imaging project](https://www.esrf.fr/home/news/general/content-news/general/esrf-and-ucl-scientists-awarded-chan-zuckerberg-initiative-grant--for-human-organ-imaging-project.html)

PaNOSC related work packages
------
* [WP2 – Data policy and stewardship](https://www.panosc.eu/work-packages/work-package-2-data-policy-and-stewardship/): Data stewardship for data policy
* [WP3 – Data catalogue services](https://www.panosc.eu/work-packages/work-package-3-data-catalog-services/): Data repository and search API
* [WP4 – Data analysis services](https://www.panosc.eu/work-packages/work-package-4-data-analysis-services/): Web interface to data portal
* [WP6 – EOSC integration](https://www.panosc.eu/work-packages/work-package-6-eosc-integration/): Download service

Contact person
------
[Andy Götz](mailto:andy.gotz@esrf.fr) (ESRF)

