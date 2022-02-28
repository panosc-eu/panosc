Use Case 29 – Run orange-pylost as a cloud service
=========================================================
Orange-pylost is a new open-source software developed for providing data analysis tools for surface optical metrology. The software is widely used by ESRF and many other European light sources for analysis of X-ray mirror metrology data, especially for the subaperture-stitching methods implemented in the software. A cloud version of the software would expand its reach to the light sources worldwide, helping new users to familiarise themselves with the software without the installation burden. For those, or for occasional users, the cloud implementation would also remove the need for a local high-performance workstation.

Main Contributors
------
* **Bharath Reddy Adapa** – software author
* **Francois Perrin**

Use Case Action Flow
------
* **Cloud** – Acquire and provide cloud infrastructure
* **Deploy** – Deploy orange-pylost software on cloud infrastructure
* **Use** – Ask users to register and use it, and provide feedback
* **Share** – Users can opt to share their workflows and data with multiple other users

Description of needs
------
A large instance for computation + medium storage in the cloud. The application runs well on a Windows 10 computer with 64GB RAM and a quad-core Intel i7-6700 CPU. No parallelisation exists in the software, but could be implemented in the future. A common storage of 1TB may be sufficient and could be expanded upon the need. Each user may be provided private and public folders to temporarily store their data.

Impacts from the implementation
------
Allows users to familiarise the software without installation. The cloud service would also serve as a stable working backup version in case of unforeseen software failures during future releases. The cloud service could also serve a vital role to analyse metrology datasets, which are too large to fit in the device memory of some of the user personal computers.

Generalisation of use case
------
The cloud service could potentially simplify cross-validation across users (e.g., mirror manufacturers and light sources) by using identical software version and workflows.

Other partners interested in this use case
------
All collaborators participating in MooNpics (http://www.calipsoplus.eu/joint-research-activities-jra/jra1-moonpics/) and Superflat (https://leaps-superflat.eu/) projects. After initial validation the software will be made accessible to other registered users outside the EU project partners. 

Resources
------
Orange pylost source code at https://gitlab.esrf.fr/moonpics_stitching_2018/orange-pylost

Contact person
------
[Raymond Barret](mailto:barrett@esrf.fr) (ESRF)
