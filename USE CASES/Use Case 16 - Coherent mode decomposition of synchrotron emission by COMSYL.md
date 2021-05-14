Use Case 16 - Coherent mode decomposition of synchrotron emission by COMSYL
=========================================================	
The radiation emitted by new low emittance storage rings, like the EBS at ESRF, is much more coherent than in the old synchrotrons. This is of great interest for many experimental techniques like X-ray photon correlation spectroscopy, coherent diffraction imaging, or ptychography. Perhaps the most efficient way to describe the partial coherence characteristics of a beam is to use the coherent mode. COMSYL [1,2] is a code developed at ESRF, that allows, without approximations, to calculate the coherent modes of an undulator beam. This code is of interest for beamline designers, as it proposes a new accurate way to treat the coherent properties of the beam [3], and has been used for simulations at ESRF beamlines [4]. It also helped to predict new features found in the synchrotron beams, such as singularities and vortices in the speckled cross-spectral density [5].

COMSYL solves a large eigenvalue problem that requires diagonalizing huge matrices. This is implemented using parallel computing (MPI) and requires the use of a cluster. COMSYL is written in python and makes extensive use of the library SLEPc, whose installation requires particular efforts. COMSYL is installed in the cluster at ESRF (SLURM and OAR).

It is proposed to provide COMSYL as a service for allowing synchrotron users to perform their calculations in a transparent way. This will certainly popularize the technique of coherent mode decomposition that could certainly benefit in many aspects the research with synchrotron radiation.

Main contributors
------
* Manuel Sanchez del Rio – COMSYL project leader, co-author,  main user
* Rainer Wilcke – COMSYL software support, installation and maintenance

Use Case Action Flow
------
* Define text case, and calculate it at ESRF cluster
* Supply COMSYL  in a container
* Install COMSYL container as a service in a PaNOSC node
* Test and document it
* Inform the users of the availability and benefits to use it

Description of needs
------
COMSYL is an innovative and important tool for simulating the coherence properties of a synchrotron beam.

Impacts from the implementation
------
The use of COMSYL is important to calculate properties of the beams emitted by new low emittance storage rings, and can help in high impact publications, such as [5]. Its availability as a service for the community could boost its use and certainly help in synchrotron research.

Generalisation of the use case
------
The implementation of COMSYL as a service could be a model of how to apply and implement as a service a large code requiring important computer resources to run. 

Resources
------
* The software is Open Source, available at https://github.com/oasys-kit/comsyl
* It is documented in M. Glass Ph. D. Thesis https://tel.archives-ouvertes.fr/tel-01664052

Other resources
------
An introduction to COMSYL was given at the OASYS schools (https://github.com/oasys-kit/oasys_school/). Slides from the last school (2019, Argonne, US) are: https://github.com/oasys-kit/oasys_school/blob/master/second/slides/pdf/Introduction_to_COMSYL.pdf

PaNOSC-related work package
------
[WP5 - Virtual Neutron and X-ray Laboratory (VINYL)](https://www.panosc.eu/work-packages/work-package-5-virtual-neutron-and-x-ray-laboratory-vinyl/)

Contact person
------
[Manuel Sanchez del Rio](mailto:mailto:srio@esrf.eu) (ESRF)

References
------
* [1] Glass, Ph. D. Thesis (2017) https://tel.archives-ouvertes.fr/tel-01664052
* [2] https://github.com/oasys-kit/comsyl
* [3] M Glass, M Sanchez del Rio (2017)  Coherent modes of X-ray beams emitted by undulators in new storage rings EPL (Europhysics Letters) 119:  3  http://dx.doi.org/10.1209/0295-5075/119/34004
* [4] M Sanchez del Rio, R Celestre, M Glass, G Pirro, J Reyes Herrera, R Barrett, J C da Silva, P Cloetens, X Shi, L Rebuffi (2019)  A hierarchical approach for modeling X-ray beamlines : application to a coherent beamline Journal of Synchrotron Radiation 26: 6. 1887-1901 http://dx.doi.org/10.1107/S160057751901213X
* [5] D M Paganin, M Sánchez del Río (2019)  Speckled cross-spectral densities and their associated correlation singularities for a modern source of partially coherent x rays Phys. Rev. A 100 4 http://dx.doi.org/10.1103/PhysRevA.100.043813

