Use Case 9 – Serial Femtosecond Crystallography Experiment Simulation (European XFEL)
=========================================================

Serial femtosecond crystallography is a powerful tool to resolve the structure of mesoscopic crystals, especially for small proteins. However, there are many complications, such as the pixel noise, unfunctional detector tiles and X-ray fluctuation, affecting the success of the experiment. By simulation with SimEx, one can predict the possible effects of the complications to help improve and validate the data analysis workflow.

Description of needs
------
The SimEx API in ViNYL package supported by PaNOSC.

Use case action flow
------
* Set up initial X-ray, detector and sample parameters.
* Run the diffraction simulation using the crystfel module integrated in SimEx.
* Change different detector geometries, noise response, respectively.
* Rerun the diffraction simulation.
* Set data analysis workflow using crystfel.
* Check the index results from different detector parameters to assess the complication effect.

Impacts from the implementation
------
It provides a tool for the users to validate their data analysis methodologies.

Generalisation of the use case
------
It can also be implemented for other SFX experiments.

Resources
------
* [Example jupyter notebook repository](https://github.com/JunCEEE/crystalProject/tree/master/src/controller/panoscDEMO)
* [SimEX on PaNOSC repository](https://github.com/PaNOSC-ViNYL/SimEx)

PaNOSC related work packages:
------
[WP5 – Virtual Neutron and X-ray Laboratory (VINYL)](https://www.panosc.eu/work-packages/work-package-5-virtual-neutron-and-x-ray-laboratory-vinyl/)

Contact person
------
[Juncheng E](mailto:juncheng.e@xfel.eu) (European XFEL)

Link to website:
------
https://www.panosc.eu/use-cases/use-case-9-serial-femtosecond-crystallography-experiment-simulation/
