#  WP6 fortnightly telco #2

19 Feb 2019 - 11H00 CET

Attendees: Andrea (CERN), Ian (STFC), Roberto & George (CERIC), Tiziana, Baptiste & 
Giuseppe (EGI), Sarah - Minutes - & Jean-François, Fabien, Stuart, Eric, Holger (ILL), Michael & Patrick (DESY), Henryk & Piotr (XFEL.EU), Christos (GÉANT), Idrissou & Alain (Soleil)

Link for the telco: https://ill.vidyocloud.com/join/pXM59qAfyX

## Agenda:

1. General organisation

    Minutes approval

    Action list

2. Presentation of FTS3 (Andrea Manzi/CERN, FTS product team coordinator)

3. Presentation of Globus (Krzysztof)

4. AOB

## Discussions:

1.1. Minutes of the last meeting has been approved

1.2. Action List (see Minutes of previous meeting)

The FitSM training organized during the EOSC-Hub week (9th of April) is offered by EOSC-Hub. 
See  https://indico.egi.eu/indico/event/4215/overview, be careful registration is opened  and seats are limited.

2. A 30 mn presentation of FTS3 has been done by Andrea Manzi

The slides are available under the same repository

https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP6%20EOSC%20Integration/PANOSC_Presentation.pptx

2.1 Discussions and QA:

What are the typical usage of FTS3 ? -> Transfert between datacenters, even multi-hop.

Do you propose a client for local computer, like Globus Online for the direct transfert to users' computer? -> Not at the moment and this is not on the roadmap.

In your slides, you mentionned the support for protocols like FTP, GSIFTP,  HTTP,  S3, GCLOUD but also the support for some storage solutions what does it mean? -> FTS3 is compatible with any storage as long as you can provide a supported access protocol. FTS3 is not dependant on the storage but on the protocol. Nevertheless some storage solution mentioned offers a direct support for these protocols.

Andrea remind us that the support for Globus Toolkit GridFTP server has ended (more information is available at https://github.com/globus/globus-toolkit/blob/globus_6_branch/support-changes.md).

How Photon and Neutron RIs could benefit from FTS3? What do we need to setup in order to transfert data between our datacenters and for example EGI services like the Jupyter one? -> you need: 
- a supported access protocol for the 2 servers
- an FTS instance (STFC is keen on offering such service for the PaN community)
- a VO (VOMS) for Role Based Authentication System (Christos announced that GÉANT will provide it as part of the current work on UmbrellaId).

VO model has to be more finely explored as the PaN RIs have a large number of small group of scientists and currently the authorization models are specific to each RI.

Andrea also announced that a work is going on for integrationg OpenID Connect in the FTS solution. A beta realase is available, production release should be available by end of 2019.

Ian invites to also look at dynafed http://lcgdm.web.cern.ch/dynafed-dynamic-federation-project

3.  Krzysztof was unavailable for this meeting, the presentation has been moved to our 4th Meeting.
