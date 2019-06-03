#  WP6 fortnightly telco #7

28th May 2019 - 11H00 CET

Attendees (18) : **Michael**, Patrick (DESY), Catalin (STFC), Marco, Carlos, Emiliano (CERIC), Tiziana, Giuseppe (EGI), Sarah - Minutes - & Jean-François, Fabien, Philippe, Eric  (ILL), Lajos (ELI-ALPS), Jérôme (ESRF), Miroslav (CESNET), Krzysztof (XFEL), Kareem (ESS).

Link for the telco: https://ill.vidyocloud.com/join/NWc9VqX5Sz


## Agenda:

1. General organisation

2. Presentation of the Jupyter infrastructure at DESY by Michael S.
5. AOB

## Discussions:

1. Short feedback on the EduTEAMS pilot and discussions that took place during the UmbrellaID meeting at PSI. The partnership and the technical solutions presented by Christos were very well received. As some organisation representatives participating to the MoU were not present, we have to proceed to a formal adoption by email. It is expected to get the results by June.

2. Michael gave an impressive presentation of the [Infrastructure/Platform/Function]-as-a-Service set up at DESY. The presentation was followed by demonstrations of the whole solution (interactive use of Jupyter running on HPC cluster, function services triggered by filesystem events, containers creation/maintenance with gitlab, Jupyter Hub using the complete services). 

[Michael's slides are available on the WP6 repository][https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP6%20EOSC%20Integration/Slides/2019-05-28%20Telco7/190528-PaNOSC-WP6-Telco.pdf]

The slides highlight a remarkable level of integration of the different elements leading scalability and to relatively simple user interfaces on complex systems. 

Key ideas that have been discussed during the meeting :

- The Apache Kaftka messaging system integrated into dCache allows to trigger events and computation functions automatically, the results being available for instance to Jupyter notebook interfaces. For example, availability of raw data on the dCache filesystem could be one of the trigger events and allow to immediately process data files.
- The function services, powered by Apache OpenWhisk, allow to decouple the processes that are tied up to the local infrastructure from those that could run on 3rd party infrastructure. This is a idea to further explore in the scope of the PaNOSC WP6 for hybrid scenario (Data provided by RIs' infrastructure and compute capacity by EGI).
- 





