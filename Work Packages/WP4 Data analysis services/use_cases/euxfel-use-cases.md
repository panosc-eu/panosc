# EuXFEL PaNOSC WP4 Use Cases

## Notebooks

Both users and facility staff at EuXFEL frequently use notebooks during their analysis.

Notebooks are used for anything from data exploration, to executing our data calibration pipeline.

Broadly speaking, notebook usecases can be split up into two categories based on the users: programmers and non-programmers.

Programmers create/change the code inside the notebooks as they work on the data. Non-programmers only execute the notebooks to look at its outputs, or use the notebooks via widgets/interactive plotting.

### PyFAI

[Same as ESRF](https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/use_cases/ESRF-use-cases.rst#pyfai)

### Calibration

The calibration pipeline at EuXFEL is executed through notebooks via nbparametrize.

In this case the notebooks are used as templates for the calibration process, the main reason notebooks are used is that they are converted into PDF reports at the end of the calibration process.

This means that there is a record of how the pipeline was run, allowing staff and users to see what the calibration did to the data, and to check if there were any issues.

Additionally, this improves the reproducibility of the calibration pipeline as all of the parameters used for the calibration are stored along with the steps taken.

### Live Data Monitoring

Some beamlines have made notebooks which hook into the live data stream and create a wide range of plots in real time. These plots cover anything from jitter in the data, so pixel value histograms, to monitoring regions of interest.

This caters to both categories of users: starting and running the notebook is very simple and can be done by anybody, and those users who know python can change what is being plotted as required.

### Tutorials/Information Sharing

Notebooks are often used to store and disseminate information between the users. For example, one user will develop some data analysis code, then they will annotate this code and add in usage instructions before placing the notebook in a shared folder.

From there others can copy the notebook and use it themselves with different datasets, or they can iterate on the notebook and improve it for others.

Some notebooks are also created by the data analysis team at EuXFEL as tutorials for how to use our software stack, and for how to do some specialised analysis if such information was requested before the beamtime.

## Hardware

Hardware requirements vary based on the work being done.

At the low end, basic first-look analysis does not require powerful machines, this is done either on a shared node on the cluster or with a full node allocated.

Medium requirements involve workloads which utilise some more resources but still do not use anywhere near a full node's worth of resources. These usually involve either more complex data exploration (e.g. azimuthal integration) but limited to single-frames instead of the entire dataset, or non-parallelised data analysis. 

High requirements involve using parallelised software which can fully utilise the node's power. This can be either software which has been specially designed with parallelisation in mind, or multiple instances of 'basic' analysis.

Very high requirements involve using something beyond a standard node, such as requesting a GPU node. So far this has only been required by software developed by EuXFEL staff, such as the calibration pipelines.

To summarise:

| Requirement | Hardware      | Usecase                | Example                        |
| ----------- | ------------- | ---------------------- | ------------------------------ |
| Low         | Minimal       | Data exploration       | Plotting detector image frames |
| Medium      | Med CPU/RAM   | Specialised analysis   | Azimuthal integration          |
| High        | High CPU/RAM  | Parallelised workloads | AI for whole run               |
| Very High   | CPU/RAM & GPU | Parallelised/GPU       | Data calibration               |

The hardware server hardware available at EuXFEL can be found on the [DESY Confluence docs](https://confluence.desy.de/display/IS/Hardware+in+the+exfel+partition); broadly speaking the servers fall into categories of:

| CPU | Threading | RAM   | GPU     |
| --- | --------- | ----- | ------- |
| 20  | 2x (40)   | 256GB | GP100GL |
| 36  | 2x (72)   | 768GB | none    |
| 40  | 2x (80)   | 512GB | none    |


