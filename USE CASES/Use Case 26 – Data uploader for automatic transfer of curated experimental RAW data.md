Use Case 26 – Data uploader for automatic transfer of curated experimental RAW data
=========================================================
Not all photon and neutron beamlines are equipped with an acquisition system which is fully integrated into the control system. This means that data is not saved into the online storage system automatically. Usually, this is due to the fact that proprietary acquisition systems are used (either because of the device manufacturer, legacy issues, or similar).

In order to end up with datasets, which can be connected to the data portal or data catalogue, the raw experimental data have to be curated. At the Italian CERIC partner facility, Elettra, the first step is saving data coming from such proprietary acquisition systems into the facility’s online storage. Once stored, the data can be equipped and linked to all the metadata and benefits from all the services provided by the user office like web access, DOI generation, etc.

The aim of the DataUploader application is to provide a simple way to upload data to the facility’s storage system (but not only). The application can be installed in both linux and windows workstation. It can be used only by authorised user (authentication is required), and has two modes of operation. The first one allows for uploading of data during acquisition, i. e., every time a data file is produced, it is immediately uploaded to the storage. The second one is used to upload all the data once the experiment is finished.

Main Contributors
------
* **Alessandro Olivo** – Software engineering, developer
* **Giuliana Tromba** – Scientist, tester
* **Matteo Amati** – Scientist, tester
* **Luca Petaccia** – Scientist, tester

Use Case Action Flow
------
* **Data acquisition** – Based on the mode of application, the experimental data can be acquired before the program execution or during the program execution.
* **Dataset definition** – Specify data file(s) and folder(s) which have to be uploaded and the dataset to which they must be associated. Add optional missing metadata such as dataset description, investigation description, etc.
* **Data monitoring (sync mode only)** – If the application is run in sync mode (i.e., during the acquisition), it will detect all the new or modified files produced by the acquisition system which refer to the dataset(s).
* **Interfacing with user office system** – Create the investigation and the dataset(s) in the user office system (if needed).
* **Uploading data** – Upload the experimental data from the workstation to the specified storage system.

Impacts from the implementation
------
Laboratories which have proprietary acquisition systems can make the experimental data accessible to the users via web using the user office platform (i.e., VUO).
Furthermore, the stored data can be curated in a centralised way (e.g., metadata harvesting, cataloguing) and made available to the EOSC community.

Generalisation of Use Case
------
The main goal is the adoption of this solution by all the CERIC-ERIC partners facilities which do not operate a centralised control system. This will allow us to match the need to have a centralized system curating experimental data during its entire life-cycle (from acquisition to archiving).

Other partners interested in this use case
------
All CERIC-ERIC partners facilities.

Resources
------
The software is a standalone application, which can be installed on both Windows and Linux workstation; it is a python application based on PyQt5, requests, simplejson and psutil modules. Furthermore, it requires an [rclone](https://rclone.org/) installation, which is a useful tool to interface to several types of storages system (e.g. webdav, s3, etc.).
The source code and the Windows auto-installer are available at https://gitlab.elettra.eu/ceric-data-uploader/datauploader

PaNOSC related work packages
------
[WP3 – Data catalogue services](https://www.panosc.eu/work-packages/work-package-3-data-catalog-services/)

Contact person
------
[Alessandro Olivo](mailto:alessandro.olivo@ceric-eric.eu) (CERIC-ERIC)
