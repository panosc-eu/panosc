Use Case 30 – VISA – Data Analysis in the Cloud
=========================================================
With the introduction of VISA (Virtual Infrastructure for Scientific Analysis) in June 2020, there has been a significant change with how scientists analyse experimental data and perform experiments at the ILL.

Using a web browser, within a couple of minutes, a researcher can get access to a high-performance and secure data analysis environment, installed with all of the scientific software a researcher needs with direct access to the experimental data. The VISA platform guarantees access to the latest software versions and tools, constantly upgrading the analysis environment and implementing new features.

In parallel to doing data analysis, VISA provides an ideal platform for performing remote experiments.  Accessible anywhere in the world with an internet connection, a scientist has the freedom to remotely pilot an experiment via the instrument control software, be it from the comfort of their own home or at their laboratory.

Often data analysis is performed as a team and as such VISA has been designed with real-time collaborations at its core. The platform makes it easy to share analysis environments between proposal team members, ILL scientists and computing experts.

Main contributors
------
* **Jamie Hall** – Technical project manager
* **Stuart Caunt** – Software Developer
* **Gregory Fanjas** – IT Infrastructure
* **Baptiste Pichot** – IT Infrastructure
* **Sylvain Ferot** – Software Developer

Use Case Action Flow
------
* **Login and virtual machine set up**: Using a web browser, a user logs into the platform (visa.ill.fr) using their ILL credentials. Once logged in, a user can create a new Virtual Machine on the ILL’s cloud infrastructure, that comes pre-configured with a fine tuned Ubuntu data analysis environment – it is as if the user was sitting in front of a data analysis workstation directly at the ILL.
* **Remote control and data analysis**: The machine has direct access to the ILL’s experimental storage, analysis procedures and scientific software (i.e., MANTID, MatLab, FullProf, LAMP etc.) which are ready to be used from the get go. They can also use Nomad Remote to pilot their experiment remotely directly inside of VISA.  There is the option of accessing a full Remote Desktop or launching a JupyterLab Notebook Environment for performing data analysis, alone or with the support of the ILL experts. Jupyter is an interactive, web based, online python environment allowing for reproducible data analysis and for sharing analysis routines.
Description of needs and generalisation of the use case
Initially developed as part of PaNOSC, VISA has been seen as a flagship product for performing remote data analysis with its benefits being widely accepted, however, the platform is not limited to Photon and Neutron facilities, it can also be used by other research domains.

Impacts from the implementation
------
VISA has played an essential role in contributing to a successful ILL user programme during the pandemic in 2020, allowing researchers to perform remote experiments and data analysis, despite travel restrictions and national lock-downs. Since then, more than 1,000 users have been using the platform and there has been a significant change with how scientists analyse experimental data and perform experiments at the ILL.

Thanks to VISA and NOMAD Remote, users can prepare and conduct their experiments from their own institutes, have access to the most widely used software for data reduction and analysis and create an environment for collaborating in real-time with their colleagues.

The platform is currently also used for training users such as learning about Mantid or Python programming for performing data analysis. In the near future, we will be opening up the platform to allow any user to use VISA to analyse open data.

Other partners interested in this use case
------
All six of the large-scale photon and neutron facilities (ILL, ESRF, ESS, ELI, XFEL, CERIC-ERIC) involved in this project are in the process of deploying the platform at their facilities. The VISA team is currently providing support and assistance in getting VISA ready for production at their facilities.

Resources
------
To contribute back to the worldwide scientific community, all VISA source code has been open sourced and the ILL is currently engaged in helping other interested institutes deploy the platform. Link to the source code: https://github.com/ILLGrenoble

If your facility is interested in VISA and would like more information, please get in contact with the VISA Team at visa@andygotz

PaNOSC related work packages
------
[WP4 – Data analysis services](https://www.panosc.eu/work-packages/work-package-4-data-analysis-services/)

Contact person
------
[Jamie Hall](mailto:hall@ill.fr) (ILL)
