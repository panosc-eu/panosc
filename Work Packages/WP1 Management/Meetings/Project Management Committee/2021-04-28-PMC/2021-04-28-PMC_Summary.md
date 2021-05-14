PaNOSC Project Management Committee meeting - 28/04/2021 
========================================================


Attendees
-------
Jordi (ESRF), Andy (ESRF), Jean-Francois (ESRF), Erwan (ILL), Jamie (ILL), Nicoletta (CERIC), Ornela (CERIC), Dario (CERIC), Teodor (ELI), Fabio (XFEL), Rudolf (ESRF), Carsten (XFEL), Thomas (ESS), Tobias (ESS) and Sophie (DESY, ExPaNDS)


Minutes
-------	

**1. New Project Officer**

Jordi reported that in the EU Portal a new project officer name has appeared. Jordi contacted the project officer (Simona) who replied. Jordi added that he and Andy are writting a reply to the Project Officer explaining the nature of the project, the WP breakdown and offering a meeting.

**2. How is PaNOSC going to engage/coordinate with EOSC Future?**

Rudolf reported that EOSC Future has started to organise itself, however the technical part (portal front end and back end) is very tricky, with specifications still to be produced. The kick-off meeting took place but was a bit unstructured.
Jordi asked Rudolf whether user requirements and input was sought to which Rudolf explained that for the moment EOSC Future is picking up documentation from EOSC Enhance and EOSC Hub about their engagment with the communities to check whether it is required to consult with the community.


**3. WP4 - Current Status, Challenges and Actions Required**

The WP4 review started with a [presentation](https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/slides/PaNOSC_WP4_review_20210428.pptx) by Andy that was followed by the Fabio's WP leader update and status report.

During his presentation Andy showed that WP4 is at the core of PaNOSC and it is the largest WP in terms of budget, with ILL being the largest contributor. Andy went on to show that in 2019 we wanted (as part of WP4) to have
* Jupyter Notebooks
* VISA
* Remote Data Analysis Portal
* HDF5 visualisation

He also showed that are many items in progress, but not many completed and highlighted the following challenges:
* finalising the backend of the portal
* finalising the frontend of the portal
* deploying the PaN Portal at all partner sites in production
* Jupyter extensions

He also poitned out that WP4 services should be in production within roughly 12 months and that would mean all partners contributing to ensure the challenges listed can be overcome. Even partners with smaller WP4 contributions can share their steups/ configuration to help out.

Fabio reported that we need all partners to have a PaN Portal instance in production and that the federated Search API is a key dependence and that it is required to focus  on solving this item.

A brief discussion followed on the frontend (demos, but not in production), challenges of the backend (needs to integrate UmbrellaId), the deployment and tecknology choice (Openstack vs Kubernetes) in which Thomas, Andy, Teodor, Fabio, Jean-François, Erwan, Jamie, Stuart and others participated. The ILL participants made clear that Openstack is working with them and after looking at Kubernetes they thought that the solution is overly complex for their current needs. 

There wasn't time for the remaining items in the agenda and it was agreed to schedule weekly meetings to enable a timely review of all WPs (there will be alternating regular PMC and WP review meetings)

-ENDS-
