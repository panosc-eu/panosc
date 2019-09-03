#  WP6 fortnightly telco #11

3rd Sep 2019 - 11H00 CET

Attendees :  Marco (CERIC), Giuseppe (EGI), Philippe, Jean-François (ILL), Tamas, Lajos (ELI-ALPS), 

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. General organisation (holidays)
2. Feedback on the work done during August (AAI, Data Transfer).
3. PaNOSC annual meeting in Trieste (4/5 Nov) 
https://indico.esrf.fr/indico/event/36/overview. Decision on an additional WP meeting.
## Discussions:

1. and 3. General organisation.

   We all agree that a 1 day face to face meeting during the PaNOSC Annual Meeting would be beneficial, and if possible have a common meeting with other WPs like WP4.

   Action: Jean-François to organise.

   We also discussed the use of GitHub for the documentation (minutes, slides, ...) vs Confluence (which is now available for PaNOSC). There was no strong opinion expressed during the meeting, Jean-François will enquire on how to proceed for the transfer of the current documents and feedback for the next meeting.

2. Current activities (feedback)
  1. Data transfer use case #1

     Philippe reported delayed on the set up of the ILL  GridFTP server. 

  2. Data transfer use case #2 (transfer for data analyses) . Following the Amsterdam meeting we had identified 3 pilots for use case #2:
    1. OneData 

    The OneData set up is describe in Giuseppe's report. The documentation is available on OneData web site: https://onedata.org/docs/index.html. Set up support will be provided by Giuseppe.

    Pilots: CERIC and ILL
    Installation support: EGI

    **Where do we stand ?**

    CERIC has set up a OneData infrastructure (OneProvider and OneZone) as reported by Marco. By the next meeting this pilot is expected to be avalibale for test. Marco and Giuseppe will interact to integrate this pilot with the EGI infra. Tests will be based on Elletra data.

    Giuseppe reported that EGI has updated the latest OneData API for the client access on their infratructures.

    2. dCache

    A distributed dCache between ILL and DESY to allow to run analysis outside ILL on data initially stored at ILL but cache-copied to DESY (dPool) if needed (as a test for now). For the pilot it is desirable to have a centos 7 server, but debian packages are also availables. 

    Pilots: ILL 
    Installation support: DESY

    **Where do we stand ?**

    ILL has set up a 100TB server and will contact DESY to set up dCache.

    3. Running test analysis remotely without caching the data.

    Data will stay locally at the RI and will be accessed for analysis through http using webdav protocols.
    (in case of Apache and in order to be able to w<rite files under the uid of the user we need one Apache server per user)

    Pilots: STFC and ILL

    **Where do we stand ?**

    no news yet (summer holidays)

    The OneData and DCache solutions require root access to the storage for the scenario where we store back analysis results to the original RI archives.  For this initial pilots RI will provide dedicated servers and storage instead of accessing directly the RIs' central archives.

  3. use case #3 (ELI)

     Birgit (ELI-BEAMS) has recently join the team and is working on this use case.

  4. AAI 

     GEANT had work on August on the set up of the eduTEAMS infra for UmbrellaId, but no news yet (summer holidays).

Next meeting: 17th September.