#  WP6 fortnightly telco #16

21th Jan 2020 - 11H00 CET

​	Next meeting : 18th of Feb 2020

Attendees :  Kareem, Marco, Jean-François, Rudolf, Christos, Michael, Miroslav 
Excused: Giuseppe

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. Information on the current activities : AAI and Data transfer (One data, user driven data transfer solution such as Globus, Archive pilot)
3. Need for AAI training?
3. Software catalogue ( https://software.pan-data.eu )

## Discussions:

1. #### AAI.

   Still working on the pilots (issue with the chosen OIDC plugin for confluence fixed).
   We are now able to authenticate users with UmbrellaID powered by EDUTeams using OIDC. 
   Nevertheless we are still in phase 1 ( EDUTeams acting as a transparent proxy ) and we miss a correct email adress to match UmbrellaID users and local confluence users.

   We are now working on a forthnigly  bases meeting (2H00). The GEANT team has been extended to 3 persons.

   Next step is connecting the ILL keycloack.

2. #### One data pilot: 

    Brief update about the current status of the Data transfer pilot (Giuseppe)

   - Task: Installation of the Oneprovider at CERIC-ERIC

   - Status: Solved

   - Description: 
              Solved an issue with Onedata SW stack during the configuration of the Oneprovider service at CERIC-ERIC.
              The resources for the current set-up include:

   - - A CERIC-ERIC virtual space in Onezone with sample datasets provided by CERIC-ERIC
     - 2 oneprovider services running at CESNET-MCC, and CERIC-ERIC           respectively
     - Initial data trasfer tests from CERIC-ERIC to CESNET-MCC and           vicecersa were successfully. 
     - The sample XXX was considered during the transfer test. 
     - Dataset was transferred in less than 1 min.
                

   

   - Task: Installation of the K8s cluster
   - Status: Solved
   - Description:
              The initial K8s cluster is composed by: 1 master node and 2 workers. Additional workers can be included afterwards.
              For the installation of the K8s cluster the EC3/IM framework [1] docker container was used. 
              The cluster is running at CESNET-MCC.
              During the configuration of the K8s cluster there was an initial issue with the RAM in the hypervisor hosting the VMs. 
              This issue should be fixed now after the VMs were moved to another hypervisor.
          
- Task: Customization of the K8s cluster to deploy the JupyterHub notebooks for the PaNOSC users
   - Status: In progress. 
   - Description:
              Installation of the K8s ngnix-ingress, nfs-provisioner are         working.
              Configured the K8s cluster to use the Let's Encrypt CA as         cert-manager
              Registered in the EGI DNSupdate service the hostname:         notebooks-panosc.fedcloud-tf.fedcloud.eu
              Install of the PaNOSC Jupyterhub notebooks in progress. 
                   This task requires some customizations since the EGI AAI         Check-In is not used.

We should be able to easily measure all of these each year (It should be part of our standard reporting for the Annual Conferences).



Additional information (Marco) :

- Need to redo the setup (get confident and documentation)
- New docker-image on docker-hub
- Replace let's encrypt certificats by Terena signed certificates 
- Demo for the next meeting.



#### GlobusOnline: 

EGI (Catalin) taken the lead on subscription discussions with GlobusOnline

Need to clarify which PaNOSC partner want a subscription (GO support, Rest APIs, Own Idp Provider, dashboard - Who is transferring what.)

Need Information from partners: 

- Interest in subscription Y/N
- When do you expect to open such service to users
- Potential volume of data transfered
- Potential nb of users



#### Data Archiving

Weekly meeting set up with Ian and Philippe

system set up, bi directional transfers achieved.

Need to: automate transfer using FTS -> Need to re install the ILL part on CentOS



#### Need for AAI training 

Which RI is interested (Keycloak + UmbrellaID) ?



#### SW catalogue (Task 6.6)

Need to start collecting requirements 

The Photon and Neutron community is using a software catalogue that not only references the analysis and simulation software in use and supported at the facilities but also provides complete examples with data sets and practical information for scientific instruments where they are used. This is an important documentation tool for facility users that we need to integrate into the EOSC, to make it more accessible to the whole scientific community interested into our open data. We have identified two main tasks:
- ***Implement in the current catalogue the missing features***, for instance docker/image registry, to meet the level of EOSC standard.
- In collaboration with the EOSC-hub, define and implement APIs that could allow its integration into the EOSC database catalogue. Selected software presented in the PaNData software catalogue and officially supported by at least one of the partners will benefit of this integration by being also referenced in the EOSC database catalogue.



