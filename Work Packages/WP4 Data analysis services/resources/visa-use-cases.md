# VISA use cases

### Actors

|Actor|Description|
|--- |--- |
|Admin|IT Staff|
|Facility Management (FM)|Directors, PaNOSC stakeholders (requiring metrics, usage, KPI...)|
|Instrument Responsible|Scientist in charge of an instrument|
|Intra-Facility Coordinator (IFC)|Coordinates the integration of different facilities into the PaNOSC data analysis cluster|
|Open Access User (OAU)|Public member wanting to analyse open data (typically with an affiliation to a research institute or university)|
|Proposal Team Member (PTM)|External user and Instrument Responsible|
|Scientist|Regroups Proposal Team Member and Open Access User|

### Scientific Use Cases

#### Accessing and searching for data

|ID|Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|1|PTM|I need to log into the portal using my institute credentials|||
|2|OAU|I do not belong to an institute but want to log in to analyse open data||AAI will be provided by the work done in WP6|
|3|Scientist|I want to be able to find data to analyse for an experiment at a given institute|||
|4|PTM|I want to access my experimental data|||
|5|PTM|I would like to know who has accessed my experimental data|||
|6|IR|I would like to know who has accessed data for my instrument|||
|7|PTM|I would like to know when a data file has been modified or created for my proposal||Maintain a history of modifications|
|8|Scientist|I want to explore/search for public analysis results|||

#### Machine management

|ID|Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|1|Scientist|I would like to request a machine that is capable of analysing the data. I would prefer not to log in again to the remote machine||The machine is created and presented to the user→ remote desktop presented to user→ the experimental data is mapped to the machine|
|2|Scientist|When I disconnect and then connect back to the machine I want||the machine state to be preserved from the previous session|
|3|Scientist|I want to be able to extend the lifetime of my machine|||
|4|Scientist|I want to be informed when a machine is going to be archived|||
|5|PTM|I want to be informed when a machine has been created to analyse my data (even if created by someone else)|||

#### Analysing data

|ID|Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|1|Scientist|I would like the data to be mounted to the file system on the machine|||
|2|Scientist|I would like to find software to analyse the data||install any softwaresystem proposes software relevant to the datascientist (or other user) proposes software|
|3|Scientist|I need to store the results of the analysis|||
|4|Scientist|I want to be able to analyse data from 10 years ago. I need the system and software to be capable or reading and analysing the data files from this period|||
|5|Scientist|I want to submit a job to a compute cluster (parallel processing cluster for example)|||
|6|Scientist|I want to install software that is not available in the software repositories (or proposed by the system)|||
|7|Scientist|I want to know if analysis is already in progress for the same proposal|||

#### Collaborations

||Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|1|Scientist|I want to be able to collaborate with a colleague to analyse data together||Screen sharingChatVideo|
|2|Scientist|While collaborating in a data analysis session I would like to take control of the analysis (keyboard and mouse input)|||
|3|PTM|I would like to invite someone to collaborate on data analysis who is not part of the proposal team||Grant access|
|4|Scientist|I would like to request to participate in the data analysis collaboration but I am not part of the proposal team||Request access|
|5|OAU|I want to be able to contact the proposal team about their data or published results|||

#### Recording/playback of data analysis

|ID|Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|1|Scientist|I want to see the analysis (process and results) made by somebody else||historical analysishistorical datafrom an analysis DOI? (machine, data, environment)replay?|
|2|Scientist|I would like to know what analysis has been performed on a particular dataset previously and by whom|||
|3|Scientist|I want to see the analysis performed on a particular dataset (eg watch a video or follow analysis actions)|||
|4|Scientist|I want to be able annotate my analysis recording so that somebody can follow more easily what I have done or jump to a particular step in the analysis||Add video editing techniques to add text/links to specific parts of the video. Show a timeline of video segments.|
|5|Scientist|I have finished analysing my data and I want make my process and results discoverable||How? Generate DOI? Pushed to metadata catalogue? Landing page? Search engines?|
|6|Scientist|I want to be able to record my voice while recording analysis processes|||
|7|Scientist|I want to follow the previous analysis performed on a particular dataset and then modify the actions or analysis parameters||nice to have!|

#### Assistance

|ID|Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|1|Scientist|I require help using my machine and require support staff / local contact to guide me.||Support staff can access the running machine (like a collaborator) and take control|
|2|Scientist|I want to find data analysis examples and tutorials||Link to WP8|

### Administrative Use Cases

|ID|Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|5|Admin|I need to be able to deploy updates without any down time||eg new web servers, new code release|
|4|Admin|I need to be able to scale the compute resources when necessary||ie increasing the resources for a given machine|
|6|Admin|I need to block users due to abuse|||
|7|Admin|I need to create a new machine for data analysis and mount the data for the analysis.||Different locations for compute resources and data? Transfer data to compute resources? Eg xfel has no compute resources so we transfer xfel data to ILL for analysis.|
|10|Admin|I want machines to be automatically archived after a given number of days after their creation.|||
|11|Admin|I want to be able to see analysis resources/state for all other facilities|||
|12|Admin|I want to monitor all activity (resources being used, number of connections) over all machines and on a particular machine||Dashboard overview and details on particular machines|
|2|Admin|I want to provision new analysis compute resources||Add new servers or memory or storage|
|8|Admin|I want to restore a machine that has been archived|||
|1|Admin|I want to see the machines states (active, suspended, archived, deleted (soft & hard)...)|||
|9|Admin|I want to see what is happening on a machine||Connect to RD silently|
|3|Admin|I want to take analysis resources offline (need to notify users)||Eg for maintenance or updates|

### FM and IFC Use Cases

|ID|Actor|Story|Description|Notes|
|--- |--- |--- |--- |--- |
|1|Facility|I want to see how many resources have been used during a given period (eg number of machines created, CPU hours, DOIs minted)||KPIs|
|2|IFC|Another institute wants to participate in Data Analysis as a Service. I would like to add another facility to the service providers||Cases:facility has data onlyfacility has compute resources onlyfacility has compute resources and data|

