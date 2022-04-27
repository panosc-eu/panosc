#  WP6 fortnightly telco #59

Tuesday 8th March 2022 - 11H00 CET

	Next meeting : Tuesday 22nd March 2022 at 11H00 CET

Attendees :  Karim, Cédric, Rudolf, Jean-François, David, Marco, Andrea, François, Fabio, Humaira Teodor, Christos
Apologies: Karim

## Agenda

- Activities update report
- Data Archiving using Echo 
- AOB

## Discussions:

### CS3Mesh Worshop Feedback 

### Activities :

- UmbrellaID: ExpanDS training will take place Thursday Mar 24, 2022
- UmbrellaID at ESS, issue with Keycloak. 
- Delay in answering request (forms by example - GEANT)
- Need public or semi public monitoring for the services 

- OneData - Complete the test from ESRF (large number of inodes) -> Integration with other storage solution (DESY) -> Evaluate VISA scenario -> Documentation -> Decision from the group as a community (ALL).

- OneData - Issue writing data back to the ESRF, a new version has been release and Andrea/Francois.
	
- CVMFS: Individual RI validation (ALL), Organisation as a community. Singularity containers in VISA through CVMFS (DESY/ESRF)
	-	ESRF is migrating its set of software to CVMFS
	-	ESRF is opening a stratum1 to internet for test by others (DESY is interested)
	-	CVMFS-CSI (on github)
	
- VISA deployment (CVMFS, GPU, Cluster access, Data Access, ...) ALL
 	- ESRF: CVMFS has been integrated into the images, NVIDIA GPU (vfio-pci, trying cyborg ), introduce a 2nd network interface for the VM ongoing. 
	- CERIC waiting for the proxmox provider
	- EGI-CESNET issues for bypassing keycloak, working on the demo instance
	- Using VISA for training
	- ESS VISA deployment - positive feedback by developpers-,Production Openstack is still work in progress. 
- EGI: based on CESNET ressources with EGI checkin, need to investtigate the auth 
- AAI: ESRF/GEANT + ?
- Cloud procurement: should be done by the end of the week.

Next meeting:

Cloud procurement
Data Archiving using Echo - Presentation by ILL during next meeting.
VISA (ESRF - EGI)
OneData - testing of the latest version
CERIC - depends on proxmox availaibility, ICAT with Keycloack
XFEL - MyDMS integration with keycloack (and UmbrellaID)

