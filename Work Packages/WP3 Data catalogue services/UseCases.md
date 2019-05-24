# Use cases

### Actors

|Actor|Description|
|--- |--- |
|Proposal Team Member (PTM)|Person involved in a proposal|
|Open Access User (OAU)|Public member wanting to analyse open data 
|Scientist|Regroups Proposal Team Member and Open Access User|
|Admin|IT Staff|
|Facility Management (FM)|Directors, PaNOSC stakeholders (requiring metrics, usage, KPI...)|


### Scientific Use Cases


|Actor|Story|Notes|
|--- |--- |--- |
|Scientist|I would like to know the states of Machine (i.e Energy) during an experiment |
|PTM|I would like to search for all metadata produced from the experiment (note that this are application specific)|
|Scientist|I would like to know the type of the software used for the analysis of data |
|Scientist|I want to be able to search for all data on water at the PanOSC facilities|
|Scientist|I would like to search for experiments/datasets by a particular metadata entitysample formulatitlescientific techniquesample type|
|Scientist|I would like to search for detector type|
|Scientist|I would like to know the instruments setup|
|Scientist|I would like to retrieve the logbook of an experiment|
|Scientist|I would like to find all experimental data associated with a proposalId or experimental number|
|Scientist|I would like to find all experimental data matching abstract/proposal text|
|Scientist|I would like to see the proposal details associated with experimental data (abstract, title, experimental dates)|
|Scientist|I would like to search for data from a particular institute / instrument|
|Scientist|I would like to search for data acquired during a particular period|
|PTM|I would like to find my own data (experimental data from my proposals)|
|OAU|I would like to request access to data (which is not open and I am not a proposal member)| At the ILL it is possible to request access (email sent to a proposal member)
|PTM|I would like to know who has requested/accessed my data|An proposal member can grant access at the ILL to users not associated with a proposal
|Scientist|I would like to know who is associated with an experiment (proposal members)|
|Scientist|I would like synonyms of techniques to be taken into account for the search results: eg Small Angle Diffraction => Small Angle Neutron Scattering & Small Angle Xray Scattering
|Scientist|I would like synonyms of components to be taken into account for the search results: eg surfactant == detergent, SDS == Sodium DodecylSulfate == SLS == Sodium Lauryl Sulfate == sodium salt of lauric acid etc
|Scientist|I would like to be able to search by CAS reference to a molecule (may be references in a proposal or experimental report)
|Scientist|I would like to be able to search in terms of q-range: ultra small angle, very small angle, medium angle, wide angle
|Scientist|I would like to be able to add new processed data to the catalogue after analysis

### Administrative Use Cases

|Actor|Story|Notes|
|--- |--- |--- |
|Admin|I would like to have access to all the data for my facility|
|Admin|I need to be able to identify the user performing the search to be able to handle access rights| eg to determine which proposals and data they have access to. If we get a request via the api to search for particular metadata entities, we need to be able to identify the user making the request to only show results for which they have valid permissions. 
|FM|I would like to know how many data requests (per site) have been made for a given period (eg for a KPI)|
|FM|I would like to know how many people have requested/searched for data|
|FM|I would like to know how much data (in bytes) has been requested/transferred for a given period|



