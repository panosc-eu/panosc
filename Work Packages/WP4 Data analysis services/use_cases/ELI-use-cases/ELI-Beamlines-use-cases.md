
# PaNOSC WP4 use cases at ELI Beamlines

Below is a list of selected **jupyter notebooks** that we are using at ELI Beamlines for data analysis/visualization purposes.

## Open `.h5`  files in  Paraview
To open `.h5` dataset in Paraview, special `.xdmf` file has to be created, this file consists of header, body and footer and it tells Paraview how to read the `.h5` dataset.

* Source code: [https://github.com/MariDani/h5-to-xdmf](https://github.com/MariDani/h5-to-xdmf)
* Binder: [https://gke.mybinder.org/v2/gh/MariDani/h5-to-xdmf/master?filepath=xdmf_from_h5.ipynb](https://gke.mybinder.org/v2/gh/MariDani/h5-to-xdmf/master?filepath=xdmf_from_h5.ipynb)

## Create VR web application

We are developing custom 3D web application for visualization of simulation data in browser with enabled VR mode. To enable smooth visualizations we preprocess the raw data to binary buffers using transformation tool via Jupyter Notebook.

<img src=ELI-use-cases/data_transform_tool.png>

Examples of visualizations

<img src=ELI-use-cases/web_app_preview.png>

## Analytical Modelling

<img src=ELI-use-cases/analytical_modeling.png>

## Analysis of PIC Simulations

<img src=ELI-use-cases/analysis_simulation.png>



