#  WP6 fortnightly telco #4

19th March 2019 - 11H00 CET

Attendees:  Brian, Catalin (STFC), (CERIC), Giuseppe (EGI), Sarah - Minutes - & Jean-François, Jamie, Stuart  (ILL),  Christos (GÉANT), Alain (Soleil), Lajos (ELI-ALPS), Andy (ESRF), Miroslav ( CESNET) 

Link for the telco: https://ill.vidyocloud.com/join/pXM59qAfyX

## Agenda:

1. General organisation

    Minutes approval (unfortunately minutes of our previous meeting are not available, it has to be postponed to the next meeting)

    EOSC-Hub week: Photon - Neutron working meeting (5H00 - 6H00 PM 10th April): confirm agenda/attendance. 

Agenda: 
Which EOSC-hub services can be interested for the PANOSC cluster project ?
EGI Jupyter Notebook service for the PANOSC community (10’)
Data management solutions to make federated data transparently accessible by computing resources running on different cloud environments (e-infrastructure, research infrastructures) (10’)
Status of the AAI integration in PANOSC (10’)
Data archiving (10’) 
Roadmap for the integration of the EOSC-hub services in the cluster project (20’)


    Action list:
    
    Data transfer use cases (Initial draft)
  https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP6%20EOSC%20Integration/DataTransferUseCases.md

​    

2. Discussions on the AAI integration use case for the Jupyter Notebook Service (powered by EGI).

    This is one of the use case mentioned above.

    Data are fetched from one of the PaNOSC RIs, results of the analysis are stored back at the same RI infrastructure. EGI is handling the Compute (Jupyter) Service. Users are authenticated with the UmbrellaID AAI proxyfied by eduTeam.

    This is probably only preliminary work, but from my point of view the objectives of this discussion should be :

    - Clear understanding of the scenario by the different actors, complete the use case to ensure mutual understanding.
    - How could it work? Identify potential solutions. Missing pieces and bottleneck to be addressed.
    - Action plan.

3. AOB

## Discussions:

Giuseppe went through the presentation he had prepared for the meeting https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP6%20EOSC%20Integration/AAI%20Integration%20use%20cases%20for%20Jupyter%20Notebook_v2-1.pptx

Most of the discussion took place regarding the diagram on slide 11.

Question: Regarding the current scenario, in the case of PaNOSC the community AAI will be powered by EduTEAMS  and the e-infra proxy is the EGI Check-in solution, both implement the AARC model. Could this chain of proxy be transparent for the Users ?

Response from GEANT: Yes, this is currently finalized in the last part of the AARC2 project. Users should not see another stop-point between the services.

Concerning EduTEAMS and UmbrellaID.org, Jean-François announced that mid May, there will be a presentation  and discussions at the UmbrellaID management meeting to approve the collaboration with EduTEAMS/GEANT. A limited pilot (not all functionalities will be implemented for this pilot) will be set in place before this meeting. It could also be useful for testing this use case.

This diagram is missing the access to the data. Data needs to be transferred from the RIs data center for being analysed on the JupytherHub and the result of the analyses need to be transfer back to the RIs Data center for preservation.  
Currently the authorisation for accessing data is handle locally at the RIs level, authentication could be local or using the community AAI umbrellaID in the case of web access. In this case Check-in will have to propagate  the user id to the RIs. It is simpler to keep this authorisation mechanism at the level of the RIs, but If necessary we could study another approach where the authorizations are propagated to the federation AAI (i.e. proposal group membership available as group management at the level of the federation) and validated at the (Jupyter) service level.

Action (Jean-François) update the diagram to reflect the current use case.

