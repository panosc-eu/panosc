#  WP6 fortnightly telco #20

Friday 14th April 2020 - 11H00 CET

​	Next meeting : 28th of March 2020

Attendees :  Marco, Jean-François, Rudolf, Christos, Andy, Ian J., Philippe


## Agenda:

1. DataHub progress (Giuseppe can't attend but he forwarded some notes)
- Review of actions
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

![OneData Pilot architecture](C:\Users\jf\Documents\GitHub\panosc\Work Packages\WP6 EOSC Integration\Materials\OneData Pilot architecture.png)

As soon as Marco will finalize the configuration of the second provider at CERIC-ERIC we can start to benchmark with the data transfer considering different data sets ranging from 10GB up to 100GB.