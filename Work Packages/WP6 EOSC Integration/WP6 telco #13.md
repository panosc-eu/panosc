#  WP6 fortnightly telco #13

15th Oct 2019 - 11H00 CET

Attendees :   

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. Annual meeting in Trieste and organisation of the group meeting (6th of Nov) - https://indico.esrf.fr/indico/event/36/

   Shared vision with WP3 and WP4

2. Information on the current activities : AAI and Data transfer (dCache, One data, user driven data transfer solution such as Globus)

3. Report being prepared by the end of November "integration of local compute resources into the EOSC cloud".

## Discussions:

Next meeting: Annual conference (4-6th Nov Trieste).



1.  Annual meeting 6th of June organisation:

   | 9H00 - 10-30 | AAI : What is umbrellaID powered by EDUTeams (Authentication + Authorisation). Identification of the needs at the SP side.  Organisation for the nest steps. | Jean-François/Christos/all |
   | ------------ | ------------------------------------------------------------ | -------------------------- |
   |              |                                                              |                            |
   |              |                                                              |                            |
   |              |                                                              |                            |
   |              |                                                              |                            |
   |              |                                                              |                            |
   |              |                                                              |                            |
   |              |                                                              |                            |

   

2. Configuration of OneZone, One provider has been deployed and the lumia (User Id Translation)

Report on data transfer ILL -> STFC. We have been trying transfers with GridFTP from ILL to STFC. We find the problem that we do not have compatible sets of certificates at both sites. After lots of copying certs around, we find that a CRL (certificate revocation list) related to ILL was considered out-of-date by the STFC server.