#  WP6 fortnightly telco #10

16th July 2019 - 11H00 CET

Attendees :  

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. General organisation (holidays)
2. Feedback on the work done during August (AAI, Data Transfer).
3. PaNOSC annual meeting in Trieste (4/5 Nov) 
https://indico.esrf.fr/indico/event/36/overview. Decision on an additional WP meeting.
## Discussions:

1. General organisation

2. Current activities (feedback)

   1. Data transfer use case #1

   2. Data transfer use case #2 (transfer for data analyses) . Following the Amsterdam meeting we had identified 3 pilots for use case #2:

      1.  OneData 

      The OneData set up is describe in Giuseppe's report. The documentation is available on OneData web site: https://onedata.org/docs/index.html. Set up support will be provided by Giuseppe.

      Pilots: CERIC and ILL
      Installation support: EGI

      **Where do we stand ?**

      2. DCache

      A distributed dCache between ILL and DESY to allow to run analysis outside ILL on data initially stored at ILL but  cache-copied to DESY (DPool) if needed (as a test for now). For the pilot it is desirable to have a centos 7 server, but debin packages are also availables. 

      Pilots: ILL 
      Installation support: DESY

      **Where do we stand ?**

      3. Running test analysis remotely without caching the data.

      Data will stay locally at the RI and will be accessed for analysis through http using webdav protocols.
      (in case of Apache and in order to be able to w<rite files under the uid of the user we need one Apache server per user)

      Pilots: STFC and ILL

      **Where do we stand ?**

 The OneData and DCache solutions require root access to the storage for the scenario where we store back analysis results to the original RI archives.  For this initial pilots RI will provide dedicated servers and storage instead of accessing directly the RIs' central archives.

			3.  use case #3 (ELI)
   			4.  AAI 



Next meeting: 17th September.