#  WP6 fortnightly telco #49

Tuesday 28th September 2021 - 11H00 CET

	Next meeting : Tuesday 12th Oct 2021 at 11H00 CET

Attendees :  Cédric, Jean-François, Rudolf,  Humaira, Marco , Andrea, Teodor, Christos, Andy
Excused: Gregory, Ian, Fabio



## Agenda

1. OneData advancement
2. CVMFS
3. VISA deployment outside of RI infrastructure
4. Deliverables and milestones due by Nov 2021
5. Review of the different activities
6. AOB

## Discussions:

**General info**

AAI

Elearning patform setup is ongoing, 

**OneData advancement**

Test form accessing data form Cesnet, caching data  and mounting the space on the notebook. Andrea will organise a dedicated meeting.
Install the OneClient on Visa https://github.com/onedata/oneclient
Client can have a cache configured.

ESRF should provide more information in tems of inodes/volume for a full production.

**CVMFS**

CERIC integration with proxmox, ESS is deploying OpenStack

**VISA deployment (on RI lan and outside of RI infrastructure)**

DESY work in progress

**Deliverables and milestones for 15th of Nov 2021 :**

MS18: Implementation of AAI integration at the level of the Identity providers
MS20: Second release of PaNOSC services, data and resources (work with WP3 and WP4)
Registering a service for a limited set of user initially shouldn't be an issue.

D6.2 : Compute cloud (ELI, EGI, ...)
This report will describe the technical work required to integrate partner compute resources into the EOSC
environment. In particular, the security aspects and organisational challenges will be analyzed.

D6.3 : AAI (ESRF, GEANT, ...)
The report will present the results of the feasibility study (Task 6.4) concerning the PaN AAI integration with EOSC
and the result of the collaboration with GÉANT concerning the implementation. A demonstration of PaNOSC
services with EOSC AAI will be presented.

*Discussion:* 

For declaring a new service to the EOSC portal, does this service need to be open for the community at large?  No I could be accepted to have a service limited to a community and if necessary progressively open it larger. 

Would it be possible for EGI to provide VISA for the general scientific community? Andrea: We can study the possibility, we should also discuss limits. Jean-François: we need first to analyse the technical needs for hosting a VISA instance outside a local RI (data access model, software/image provisioning, ...). Rudolf: Could also be an interesting use case for EGI-ACE. Fabio will discuss this option within WP4 and we will re-discuss it during next meeting.

**Ongoing activities**

Cloud procurement

AAI

OneData 

CVMFS

EOSC Portal service registration

 

WP8 organise the 8th and 9th November a workshop,  Best practice (lessons learnt) on data operation / stewardship. 
