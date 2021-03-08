Use Case 7 – Data Transfer using EGI-DataHub/Onedata (CERIC-ERIC)
=========================================================

Until recently, most Neutron and X-ray (Photon and Neutron also known as PaN) facility users had to use predominantly portable media to transfer data produced by the research infrastructure’s (RI) instruments to their home lab for analyses. This was the predominant model some years ago, when the volume of data was relatively low and compatible with the network, the storage and the compute capacity of the facility users’ organisations.

Nowadays, the volume of the raw data produced for a single experiment in a photon or neutron RI ranges from some hundreds of MB to 100 TB depending on the instrument technique. This 106-scale factor, associated with the large spectrum of scientific communities with very diverse practices makes it extremely difficult to propose a single model for the scientists that want to process data.

In this use case, a data transfer solution using EGI-DataHub/OneData is showcased, for users willing to analyse datasets produced during one of the experiments at a PaN RI, using the Jupyter Notebooks service in the EGI infrastructure.

Use case action flow
------
*Transfer data via EGI DataHub based on Onedata from an NFS storage located at CERIC-ERIC / Elettra RI to EGI infrastructure Data Analysis service
*Archive the results back to the originated RI
*Authenticate users using the EOSC ready PaN community AAI (UmbrellaID)

Impacts from the implementation
------
*ata transfer of up to 100 GB
*HDF5 data files >1GB can reach the maximum bandwidth available
*Smaller files have a much smaller throughputs (1/5)
*Files<50MB in size take the same amount of time of 250MB files, probably to the overhead required by the Onedata transfer protocol, a standard pattern of network file transfer protocols.

Partners
------
All synchrotons interested in analysing data using cloud resources & jupyter notebook.

Generalisation of Use Case
------
The pilot may be extended deploying Oneprovider and a PaNOSC Space for each RI.

Resources
------
EGI Notebooks service for supporting big data analytics
EGI DataHub/Onedata for federating data sets from the PaNOSC RIs
UmbrellaID as community AAI proxy for the PaNOSC community

Other resources
------
[Data transfer pilot on Github](https://github.com/EGI-Foundation/data-transfer-pilot)
[PaNOSC D6.1 Data-Hub](https://www.panosc.eu/wp-content/uploads/2020/12/D6.1_DataHub.pdf)
[PaNOSC data transfer pilot setup](https://documents.egi.eu/public/ShowDocument?docid=3686)
[EGI DataHub](https://docs.egi.eu/users/datahub/)
[EGI Notebooks service](https://www.egi.eu/services/notebooks/)

PaNOSC related work packages:
------
[WP6 – EOSC integration](https://www.panosc.eu/work-packages/work-package-6-eosc-integration/)

Contact person:
------
[Marco De Simone](mailto:marco.desimone@ceric-eric.eu) (CERIC-ERIC)

Link to website: 
------
https://www.panosc.eu/use-cases/use-case-7-data-transfer-using-egi-datahub-onedata/
