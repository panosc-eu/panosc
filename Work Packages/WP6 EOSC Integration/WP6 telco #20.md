#  WP6 fortnightly telco #20

Friday 14th April 2020 - 11H00 CET

​	Next meeting : 28th of April 2020 at 11H00 CET

Attendees :  Marco, Jean-François, Rudolf, Christos, Andy, Ian J., Philippe
Giuseppe (excused, sent his notes)


## Agenda:

1. DataHub progress (Giuseppe can't attend but he forwarded some notes)
2. Review of actions
3. AOB

## Discussions:

This week CYFRONET released a new version of the fs.onedatafs-19.02.1.1 libraries to solve the
problem Giuseppe had with reading .hd5f file remotely from the Onedata volume space.

Thanks to this fix he managed to create a first notebook that:

- Read the .hdf5 data sets from the CERIC-ERIC provider
- Process the data sets with the notebook installed at CESNET-MCC
- Upload the result (an image) of the analysis from the notebook back to the CESNET-MCC provider
- Trigger the upload of the image to a second one-provider at CERIC-ERIC via APIs

The full workflow is described in this high-level architecture:

![](https://raw.githubusercontent.com/panosc-eu/panosc/master/Work%20Packages/WP6%20EOSC%20Integration/Materials/OneData%20Pilot%20architecture.png)

As soon as Marco will finalize the configuration of the second provider at CERIC-ERIC we can start to benchmark with the data transfer considering different data sets ranging from 10GB up to 100GB.

A discussion follow on the level of maturity of the solution. The regular need of patches to achieve this setup was a bit surprising, after the meeting  I realized that these patches concerns  mostly a filesystem abstraction library (ONEDATAFS) for Python (in the case of Jupyter), which is a fairly recent development and come in addition to the POSIX access functionality to data.

Action 1: Marco to inform before the next meeting  if the benchmark will be possible for the current deliverable.
Action 2: Jean-François to generate the certificate for the UmbrellaID proxy environment.
Action 3: Philippe to modify the ILL proxy config to allow FTS to be used from the ILL network.
Action 4: Andy ask if the UKRI ressources currently used for the test with ILL could also be used for ESRF archiving, Ian should check.