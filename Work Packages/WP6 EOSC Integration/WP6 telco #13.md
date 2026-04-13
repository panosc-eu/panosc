#  WP6 fortnightly telco #13

15th Oct 2019 - 11H00 CET

Attendees :   Giuseppe (EGI), Jean-François (ILL), Lajos (ELI), Ian (STFC), Brian (ESS)

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. Annual meeting in Trieste and organisation of the group meeting (6th of Nov) - https://indico.esrf.fr/indico/event/36/

   Shared vision with WP3 and WP4

2. Information on the current activities : AAI and Data transfer (dCache, One data, user driven data transfer solution such as Globus)

3. Report being prepared by the end of November "integration of local compute resources into the EOSC cloud".

## Discussions:

Next meeting: Annual conference (4-6th Nov Trieste).



1.  Annual meeting 6th of June organisation:

   | Timeslot      | theme                                                        | Preparation                           |
   | ------------- | ------------------------------------------------------------ | ------------------------------------- |
   | 9H00 - 10-30  | AAI : What is umbrellaID powered by EDUTeams (Authentication + Authorisation). Identification of the needs at the service side (RIs).  Organisation for the nest steps. | Jean-François/Christos/all            |
   |               | Break                                                        |                                       |
   | 10H45 - 12H30 | Data transfer: OneData, dCache, ... Results of the initial pilots | All involved in the pilots activities |
   |               | Lunch                                                        |                                       |
   | 14H00 - 16H00 | Joint meeting with WP3 and WP4 - Vision / respective needs   | All                                   |
   |               | Coffee                                                       |                                       |
   | 16H15 - 17H00 | Work in common on the report.                                | All                                   |

   

2. Current activities

   AAI: Pilot has been set up with only the UmbrellaID Idp (EduGAIN and ORCID will be introduced in the 2 step). Fisrt SP to be setup this week, demo at the user meeting.

   Configuration of OneZone done. One provider has been deployed with lumia (User Id Translation) at CERIC. Reported by Giuseppe.

   Report on data transfer ILL -> STFC. We have been trying transfers with GridFTP from ILL to STFC. We find the problem that we do not have compatible sets of certificates at both sites. After lots of copying certs around, we find that a CRL (certificate revocation list) related to ILL was considered out-of-date by the STFC server. Update 30/10/19: In fact, it was the client (ILL) which had an out-of-date CRL for the UK eScience CA. Ian Johnson provided a in-date CRL to ILL. This allowed the transfer to proceed further than before; the remote user (Holger) was authenticated OK, write permission to the destination file was agreed, but the transfer got a 'handshake error' before the transfer of data could start. Ian is still investigating.

3.  Discussion on the report, it will be based on the use of services.

4. Giuseppe talk about the presentation do,ne by EGI at EaPEC 2019. Slides are available at https://documents.egi.eu/public/ShowDocument?docid=3515 and a video is available at https://www.youtube.com/watch?v=ODv592Uzja4
