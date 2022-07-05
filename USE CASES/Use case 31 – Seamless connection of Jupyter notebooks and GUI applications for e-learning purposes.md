Use case 31 – Seamless connection of Jupyter notebooks and GUI applications for e-learning purposes
=========================================================
Open education through MOOCs (massive open online courses) has attracted considerable attention in recent years, both due to availability in technology, and to a recent increase in demand for online content. The PaN e-learning platform is a portal which represents the joint effort of the PaN community. The PaNOSC and ExPaNDS projects have been building it on the legacy of the e-neutrons.org portal, offering complete courses for training of the next generation of photon and neutron users. The system itself has been built on the Moodle platform, which provides the whole package of course, evaluation and content creation. However, for the courses to be suitable for the PaN community, one needs remote access to the data analysis services. One solution is to use Jupyter notebooks, which are easily accessible through an instance of Jupyter Hub. But this does not solve the problem with workflows, which rely on software with graphical user interface (GUI).

The use case described here has stemmed entirely from PaNOSC collaboration. The system will be primarily used for teaching at the PaNOSC Summer School. It combines work from multiple PaNOSC partners and serves the software developed by the partners involved in PaNOSC.

To address this and provide seamless access to GUI programs from the PaN-learning platform, Panosc partners CERIC-ERIC and ESS have selected a solution where the desktop is instantiated and run through Jupyter Hub. For this, we have forked the following project: https://github.com/yuvipanda/jupyter-desktop-server, which served as the tech stack base, and populated it with our own set of PaN software tools. The Docker container can be exploited for use in individual courses, or as a complete package. This will be the case in the upcoming PaNOSC Summer School, where students will interact with the website in a seamless way, thus avoiding the need to install and maintain any specific programs. The user simply logs-in into the Moodle portal and clicks on the Jupyter Hub icon. Then, they can open the XFCE desktop from a drop-down menu in a new browser tab. The credentials and authentication for the user are shared.

Main contributors
------
* **Marco De Simone** (CERIC-ERIC) – Proof-of-concept of the specific Docker container
* **Aljosa Hafner** (CERIC-ERIC) – Initiator, specification provision and beta testing 
* **Peter Willendrup** (DTU and ESS) – Development and deployment of the final Docker container

Generalisation of the use case
------
Even though the Docker container in its current form and use case is intended for use in training, there are no obstacles to deploy GUI programs as remote services for use in the actual development/production environment.

Other partners interested in this use case
------
All PaNOSC partners may capitalise on the use case, and specifically ESRF and ELI-ERIC, who are directly involved in the programme of the PaNOSC Summer School 2022.

Resources
------
* **Code repository**: https://github.com/pan-training/Docker/tree/main/wp8-summerschool
* **Docker image**: https://hub.docker.com/r/mccode/panosc-summerschool-0.1
* **McStas**: neutron instrument- and experiment simulations
* **OASYS**: X-ray optics and beam-line simulations
* **Crispy**: core-level spectra calculator – ASE: Atomic Simulation Environment

PaNOSC related work packages
------
* [WP5 – Virtual Neutron and X-ray Laboratory (VINYL)](https://www.panosc.eu/work-packages/work-package-5-virtual-neutron-and-x-ray-laboratory-vinyl/)
* [WP8 – Staff and user training](https://www.panosc.eu/work-packages/work-package-8-staff-and-user-training/)

Contact person
------
[Aljoša Hafner](mailto:aljosa.hafner@ceric-eric.eu) (CERIC-ERIC)
