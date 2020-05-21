# KPIs

## Definitions

- KPIs are defined during Trieste meeting ([https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/Meetings/2019-11-04-Trieste/notes.org#kpis](https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/Meetings/2019-11-04-Trieste/notes.org#kpis))

- They are
  - KPI1: Percentage of facilities offering JupyterHub or remote desktop for analysis services
  - KPI2: Number of unique users making use of JupyterHub or remote desktop for analysis services at partner facilities
  - KPI3: Number of “techniques” available through remote services

  ## Required data:
  
  We need to find the corresponding numbers from every facility from
  - (old) before the project started, i.e. month0 (=M0) and
  - (old) after the first year, i.e. on 30 November 2019, (=M12)
  - (new) a snapshot from beginning of May 2020 (=M17)

|            |  KPI1 M0 | KPI 1 M12               | KPI1 M17               | KPI 2 M0 | KPI 2 M12 | KPI2 M17 |   KPI 3 M0 |   KPI 3 M12 | KPI3 M17 |
| ---------- | -------- | ----------------------- | ---------------------- | -------- | --------- | -------- | ---------- | ----------- | ----------- |
| CERIC-ERIC |        0 | (JupyterHub)            |                        |        0 |         0 |          |          0 |           0 |             |
| ELI        |        0 |                     -   | (JupyterHub)           |        0 |         1 |        2 |          0 |           1 |           1 |
| ESS        |        1 | (JupyterHub/VNC)        | (JupyterHub/VNC)       |       10 |        20 |       40 |          1 |           1 |           1 |
| EuXEL      |        1 | (JupyterHub/FastX)      | (JupyterHub/FastX)     |        - |       150 |  150-200 |          2 |           2 | 2           |
| ESRF       |        1 | (JupyterHub/NoMachine)  | (JupyterHub/NoMachine) |       20 |         0 |        0 | 1 beamline | 3 beamlines | 3 beamlines |
| ILL        |        1 | (JupyterHub/VISA)       | (JupyterHub/VISA)      |        0 |         1 |          |          0 |           2 | 40 instruments (remote desktop and jupyter) |
