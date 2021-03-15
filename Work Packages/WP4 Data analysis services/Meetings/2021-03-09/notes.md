# WP4 Monthly meeting March 2021 - minutes

2021/03/09

The meeting follows the proposed agenda, distributed beforehand

## Work-package leadership

- Sandor Brockhauser (SB) announces the end of his role as WP4 leader,
  introduces Fabio Dall'Antonia (FD) as successor

## Portal naming

- SB announces the renaming of PaNOSC portal to PaN portal, since
  - it was developed in collaboration with the ExPANDS project
  - shall not be restricted to the PaNOSC project (its purposes, scope or duration)
  - shall be inclusive to the overall photon and neutron science community.

- ILL asks for options to change the proposed name, this question is left open


## Reports from the portal development task force

ILL:
- will continue on microservices work next week
- summarize developments in the last months:
  - documentation of the architecture
  - account service
  - orchestration of microservices
  - pipeline

CERIC:
- logging service commited to Gitlab
- as follow-up of a meeting with Stuart [ SURNAME? ] will start integrating that service into the portal

EuXFEL:
- integration of the Jupyter-SLURM provider to the portal was archieved in a more straight-forward
  manner, "tricks" like a local demon are not any more required
- the JupyterHub installation will be front-end with SLURM integration at the back-end,
  DESY is working on the integration of the two
- tokens from the portal can be taken over by JupyterHub (to be tested by DESY colleagues)

ELI:
- Jiri Meyer (JM) reports on UI development.
  - implementation not yet complete, recommends to use dev branch from Gitlab
  - Teodor Ivanoica (TI) proposes demo of operational code with discussion at next development meeting
- Andy Goetz (AG) asks which hardware for production environment is recommeded
  - ELI will present their environment and tests at that next dev meeting,
    likewise Michael Schuh for DESY

- SB's suggestion for search API demonstrator deliverable: include a screenshot of the UI


## Reports from the use case task force

EuXFEL (FD):
- XGM data from pulse delivery studies
- ML on shock-wave spectra
- detector calibration
- NeXUS master file generation from SFX data

ESRF (Thomas Vincent):
- pyNix [?] / PyFAI use case, tutorial for azimuthal integration
- on use case corresponding to scientific data from user
  who did notebook-based analysis and published data with notebooks

ILL:
- cannot present scientific use cases currently
- SB remembers video on remote experiments
- AG emphasizes value of any "user story" on real-life data
  (there are many such stories, just speak to scientists)

ELI (TI):
- one use case was shown in a presentation
- they have another one from last year
- one more yet to come

CERIC:
- Andrea Lorenzon states that a bit more time is needed
- SB asks if more details could be given next months, this is affirmed

ExPANDS:
- Chris Reynolds mentions use case from DLS with link shared
- points out limited portability if part of dependencies are in a container, 
  but others not
- SB referes to Robert Rosca (RR) about scenarios where notebooks can "re-create" their data
  by fetching from somewhere - RR mentions myBinder with hooks
  - postBuild: runs code after installing the environment, changes made by this are saved
    in the docker image created and used by binder
  - start: code getting executed every time a binder session starts up, useful for downloading
    or decompressing data we want to provide to users
- Krisztian Pozsa highlights Jupyter notebook showcase for a review meeting,
  about tomographic data processing, and the ease with which this can be used
  from different infrastructural framework (DESY & other)

## Milestones

- Next major milestone for month 42
- closer internal milestones
  - KPI snapshots end of May (collecting statistics for indicator numbers)
  - PaN portal version 2: should include all features currently worked on and partly
    discussed today

## AOB

- RR announces leaving PaNOSC
  - AG asks if the "notebook competition" inititated by RR goes on nonetheless. RR: in principle yes
- ELI (TI) aims at replacing some mock-up use case data with more realistic examples in order
  to attract users
