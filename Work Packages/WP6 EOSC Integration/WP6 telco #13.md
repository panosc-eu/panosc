#  WP6 fortnightly telco #13

15th Oct 2019 - 11H00 CET

Attendees :   Giuseppe (EGI), Jean-François (ILL), Lazlo (ELI), Ian (STFC), BRIAN (ESS)

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. Annual meeting in Trieste and organisation of the group meeting (6th of Nov) - https://indico.esrf.fr/indico/event/36/

   Shared vision with WP3 and WP4

2. Information on the current activities : AAI and Data transfer (dCache, One data, user driven data transfer solution such as Globus)

3. Report being prepared by the end of November "integration of local compute resources into the EOSC cloud".

## Discussions:

Next meeting: Annual conference (4-6th Nov Trieste).



1.  Annual meeting 6th of June organisation:

   | 9H00 - 10-30  | AAI : What is umbrellaID powered by EDUTeams (Authentication + Authorisation). Identification of the needs at the service side (RIs).  Organisation for the nest steps. | Jean-François/Christos/all            |
   | ------------- | ------------------------------------------------------------ | ------------------------------------- |
   |               | Break                                                        |                                       |
   | 10H45 - 12H30 | Data transfer: OneData, dCache, ... Results of the initial pilots | All involved in the pilots activities |
   |               | Lunch                                                        |                                       |
   | 14H00 - 16H00 | Joint meeting with WP3 and WP4 - Vision / respective needs   | All                                   |
   |               | Coffee                                                       |                                       |
   | 16H15 - 17H00 | Work on the report.                                          | All                                   |
   |               |                                                              |                                       |

   

2. Current activities

   AAI: Pilot set up with only the UmbrellaID Idp. Fisrt SP to be setup this week, demo at the user meeting.

   Status of the 2nd. pilot: "Remote Data analyses using Jupyter notebook services of another provider"
   - The CESNET-MCC allocated the resources for hosting no.1 instance of Onezone (release v18.02.1). 
   - CERIC-ERIC is finalizing the configuration and the installation of no.1 instance of Oneprovider with LUMIA support 
     for the UserId translation.
   - A new release of Onedata (v19.02.1) has been rolled-out into production on 14/10/2019   

   Report on data transfer ILL -> STFC. We have been trying transfers with GridFTP from ILL to STFC. We find the problem that we do not have compatible sets of certificates at both sites. After lots of copying certs around, we find that a CRL (certificate revocation list) related to ILL was considered out-of-date by the STFC server.

3.  Discussion on the report, it will be based on the use of services like Jupyter.

4. Giuseppe reported about the tutorial organzied by EGI at EaPEC 2019. 
   Slides are available at http://go.egi.eu/eapec2019 and video at https://www.youtube.com/watch?v=ODv592Uzja4
