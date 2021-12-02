Use case 27 – CCP4 cloud service for MX
=========================================================
The [CCP4 software](https://www.ccp4.ac.uk/) is a widely used software suite for doing molecular replacement for protein structures. It offers the software services required by scientists doing macromolecular crystallography after taking data at a photon source, e.g. synchrotrons. The aim of this use case is to deploy the cloud version of CCP4.

Main Contributors
------
* **Francois Sturma** – Cloud system support
* **Gianluca Santoni** – Scientist – expert user in CCP4
* **Eugene Krissinel** – CCP4 developer
* **Giuseppe La Rocca** – EGI systems support

Use Case Action Flow
------
* **Cloud** – Acquire and provision cloud infrastructure
* **Deploy** – Deploy CCP4 suite on cloud infrastructure
* **Use** – Ask users to register and use and provide feedback
* **AAI** – Integrate support for UmbrellaID for AAI

Description of needs
------
A large instance for computation + medium storage in the cloud.

Storage: the current DLS install has 5Gb per user, giving space for 2 reasonably sized projects CPU: needs discussion as most tasks require 1cpu, but a few would take advantage of higher parallelisation. Is 200 CPUs a reasonable request?

Impacts from the implementation
------
Autoprocessing pipelines provided at the beamline stop about half way through the process of deposition of a structure into the [Protein Data Bank (PDB)](https://www.rcsb.org/). Users then keep processing their data at home, after downloading the results we provide. With the CCP4cloud install we could:

* Limit the data transferred from and to the ESRF
* Provide resources automated model building pipelines, removing the duty of managing local installations of complex software for the users, as well as limiting the amount of computing resources acquired by each single research group. Centralised systems are more cost effective as the downtime should be minimal.
* Have a finer control of the published experimental metadata, as we can have a direct link (pull from ccp4cloud) with the ISPyB database
* The estimated user community of CCP4 is of around 25 thousand research groups around the world. Europe represents roughly half of it.

Generalisation of the use case
------
The CCP4 cloud suite has currently 50 000 registered users. Providing CCP4 as part of EOSC is potentially useful for this community.

Other partners interested in this use case
------
ALL partners doing MX – EUXFEL, CERIC-ERIC

Resources
------
https://www.ccp4.ac.uk/download/
AWS – Cloud resources for running the CCP4 suite

PaNOSC related work packages
------
[WP6 – EOSC integration](https://www.panosc.eu/work-packages/work-package-6-eosc-integration/): Cloud resources – commercial and EOSC


Contact person
------
[Andy Götz](mailto:andy.gotz@esrf.fr) (ESRF)
