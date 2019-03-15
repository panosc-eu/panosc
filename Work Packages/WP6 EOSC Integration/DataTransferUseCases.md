# Data transfer use cases  (Preliminary draft)



## Remote archive of a facility experimental data

**Story**

This is a relatively simple use case:s a PaNOSC user facility wants to get a cold archive of the experimental data produced on its premises.

Initial transfer is in the order of 600TB, the annual volume of data that should be transfered is in the order of 300TB. (it could vary up to 10PB for some facailities).

The facility needs the possibility to retrieve data on demand (in case of failure of its internal/primary storage)

**Actors**: The user facility and the archive provider ( a second, more complex, scenario could further extend this list to the facility users and other service provider )

**Potential constraints**:



## Remote Data analyses using Jupyter notebook services of   another provider (EGI in this particular case)

**Story**

A scientist wants to perform analysis on data sets obtained during an experiment at one of the PaNOSC RIs. 

The compute and data infrastructure are distant.

The scientist should be able to get his data from the RIs and store back the results at the same facility.
Datasets are still under embargo, which means that the data at the facility could only be accessed by a user  with the sufficient authorizations (the user has to be part of the proposal team).

The RIs offers a service to host the results of the analyses, but the user could decide to host the data elsewhere under his own responsibility.

**Actors**: The user facility holding the data, the user performing the analysis, the Jupyter service provider.

**Potential constraints**:



## Remote Data analyses using Jupyter notebook services of   another provider (EGI in this particular case)

**Story**

A scientist wants to perform analysis on data sets obtained during an experiment at one of the PaNOSC RIs. 

The compute and data infrastructure are distant.

The scientist should be able to get his data from the RIs and store back the results at the same facility.
Datasets are still under embargo, which means that the data at the facility could only be accessed by a user  with the sufficient authorizations (the user has to be part of the proposal team).

The RIs offers a service to host the results of the analyses, but the user could decide to host the data elsewhere under his own responsibility.

**Actors**: The user facility holding the data, the user performing the analysis, the Jupyter service provider.

**Potential constraints**:



## User's data transfer to its home organization/home computer.

**Story:**

A facility users wants to transfer his data to its home organisation or home computer.

The volume of data (up to 100TB) is important and he has difficulty to ensure this transfer in a one go.

The user needs a simple tool that will ensure the complete transfer without having to resume it himself. 

**Actors**: The user facility holding the data, the user performing the transfert.

**Potential constraints**:

