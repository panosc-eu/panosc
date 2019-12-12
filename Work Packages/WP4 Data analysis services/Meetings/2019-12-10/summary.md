# WP4 Video meeting <2019-12-10 Tue 15:00>

# Attendees

- Stuart (ILL), Jamie (ILL), William (ILL), Eric (ILL)
- Thomas (ESRF), Jerome (ESRF), Aidan (ESRF)
- Jakub (ELI)
- Lottie (ESS), Kareem (ESS)
- Robert (XFEL)

# KPIs

- KPIs are defined during Trieste meeting ([https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/Meetings/2019-11-04-Trieste/notes.org#kpis](https://github.com/panosc-eu/panosc/blob/master/Work Packages/WP4 Data analysis services/Meetings/2019-11-04-Trieste/notes.org#kpis))
- They are
  - KPI1: Percentage of facilities offering JupyterHub or remote desktop for analysis services
  - KPI2: Number of unique users making use of JupyterHub or remote desktop for analysis services at partner facilities
  - KPI3: Number of “techniques” available through remote services
- We need to find the corresponding numbers from every facility from
  - before the project started, i.e. month0 (=M0) and
  - after the first year, i.e. on 30 November 2019, (=M12)

| KPI 1 M0   | KPI 1 M12                | KPI 2 M0 | KPI 2 M12 | KPI 3 M0   | KPI 3 M12   |
| ---------- | ------------------------ | -------- | --------- | ---------- | ----------- |
| CERIC-ERIC |                          |          |           |            |             |
| ELI        | 0                        | 0        | 0         | 0          | 1           |
| ESS        | 1 (JupyterHub)           | 0        | 0         | 0          | 0           |
| EuXEL      | 1 (JupyterHub/FastX)     | -        | 150       | 2          | 2           |
| ESRF       | 1 (JupyterHub/NoMachine) | 20       | 0         | 1 beamline | 3 beamlines |
| ILL        | 1 (JupyterHub/VISA)      | 0        | 1         | 0          | 2           |

# Next meetings

## Video meeting

14 January 2020, 15:00 ([https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/Meetings/2020-01-14/notes.org](https://github.com/panosc-eu/panosc/blob/master/Work Packages/WP4 Data analysis services/Meetings/2020-01-14/notes.org))

## In person

- what weeks would be sensible?
  - Ideally in March (2020)
- Probably soon after portal release?
- who could host?
  - ESRF have offered to host the next meeting (ILL can also contribute if extra help is needed)
- It was discussed to host smaller meetings dedicated to individual topics. ESRF suggested a joint meeting between HDF viewer developers  and portal developers. The focus on these smaller meetings would be technical & hands-on i.e. coding together on certain tasks. ILL  proposed that it could organise a first meeting in February (ESRF have two new hires for PaNOSC at this time).

# Update from Portal (Jamie/Stuart)

ILL started working on the portal development approximately ~4 weeks ago. The main focus has been on the development of the [cloud-provider-kubernetes](https://github.com/panosc-portal/cloud-provider-kubernetes) micro-service.  Documentation for this service can be found here:  https://confluence.panosc.eu/x/1gCm. The development of this micro-service should be finished next week. After this, work will start to begin on developing the cloud service.


# Progress reports from each site

**ELI**

Hiring a new person to start in January.  Back-end and front-end development to work on the portal.

**ESS**

Time was spent last week running security checks on Jupyterhub preparing it for access to the outside world ready for users.

**ESRF**

Currently in discussion with scientists to get information about pertinent analysis use cases.

XFEL

Work is being done on acquiring a new JupyterHub service based on a different cluster. Hope to be made available in February.  Working on more interface Jupyter tools. Investigating using Singularity inside Kubernetes instead of docker for the notebook containers.

ESRF

Aidan has been working on finalising the SLURM integration inside Jupyter.  They are currently waiting for a production ready cluster.

ILL

Continued to work on provisioning a JupyterHub targeting IN5 (instrument). This is the candidate instrument for testing and acquiring feedback this service. This also includes data analysis templates (i.e. integration ILL data analysis tools inside the notebook). Portal development continued.


# Any other business

------

Hiring updates:

ELI (new hire in January)

ESRF  (2 new hires starting in February)


# Future topics

- Report from reproducible studies
- REANA
- Training material

