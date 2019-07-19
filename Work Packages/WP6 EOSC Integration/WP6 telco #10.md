#  WP6 fortnightly telco #10

16th June 2019 - 11H00 CET

Attendees : Marco (CERIC), Giuseppe (EGI), Jean-François (ILL), Idrissou (Soleil), Ian (STFC), Michael, Paul (DESY), Tamas (ELI), Miroslav (CESNET).

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. General organisation (holidays)

2. Report on the Amsterdam meeting
   
   Two reports are available:
   
   Giuseppe: https://docs.google.com/document/d/1QiYOAjUbzAXptulnWfc5BF2jA3MK5rWEZSz__rqMzS0
   Bjorn: https://docs.google.com/document/d/1RdbPhzudmpApeX7k6jJCGaTA4eNT7ogS11AEUY2k6gM/edit#heading=h.54v2q18nga5u
   
3. Clarify on the RI side who is ready to engage in the technical tasks (and when).

4. Ongoing recruitments and related difficulties if any.
## Discussions:

Discussion have focus on the 2nd use case as describe in the use cases document (needs to be updated) https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP6%20EOSC%20Integration/DataTransferUseCases.md.

Following the Amsterdam meeting we have identified 3 pilots for use case #2:

1) OneData 

The OneData set up is describe in Giuseppe's report. The documentation is available on OneData web site: https://onedata.org/docs/index.html. Set up support will be provided by Giuseppe.

Pilots: CERIC and ILL
Installation support: EGI

2) DCache

A distributed dCache between ILL and DESY to allow to run analysis outside ILL on data initially stored at ILL but  cache-copied to DESY (DPool) if needed (as a test for now).

Pilots: ILL
Installation support: DESY

3) Running test analysis remotely without cache the data.

Data will stay locally at the RI and will be accessed for analysis through http using webdav protocols.
(in case of Apache and in order to be able to w<rite files under the uid of the user we need one Apache server per user)

Pilots: STFC and ILL

 The OneData and DCache solutions require root access to the storage for the scenario where we store back analysis results to the original RI archives.  For this initial pilots RI will provide dedicated servers and storage instead of accessing directly the RIs' central archives.

Actions: 

CERIC and ILL should prepare a server for September
All should update/comment in order to improve  the use case description



Next meeting: 3rd September.