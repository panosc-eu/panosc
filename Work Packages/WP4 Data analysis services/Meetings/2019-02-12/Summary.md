# Minutes

#### Participants


Jamie (ILL), Stuart (ILL), Eric (ILL), Fabien (ILL), Hans (XFEL),   Robert (XFEL),  Thomas (ESRF), Jerome (ESRF), Jakub (ELI), Marianna (ELI), Lottie (ESS)      

#### Agenda      
 - Update on previous meetings actions (5 to 10 min)
    - *ESRF are  advanced in terms of Jupyter usage*
    - *Currently testing on the Amazon cloud using Jupyter notebooks and Guacamole. No OpenGL for the moment.* 
    - *Using PyFAI inside Jupyter notebooks. Presentation: https://indico.esrf.fr/indico/event/22/session/3/contribution/4/material/slides/1.pdf*
    - *Using https://pypi.org/project/crispy/*
 - Identify and contact at least three keys users for each institute 
     - *Still a work in progress* 
- Deploy a JupyterLab instance at each institute
    - *ESRF already has a JupyterLab instance being used on 6 beam lines* 
- Complete the institute survey
    - *Waiting for all partners to complete. Feedback will be given at the next meeting (26 Feb 2019)*      
- Create google docs for KPIs and Risks      
    - KPIs document      
    - Risks document      
      - *It was agreed that it was not very urgent for the moment. A qualitative value will be added by Hans.*
- Create a google doc for Task 4.1 survey
    - *Nothing to report*
- Define working groups
    - *We agreed it would be good to create two separate channels on Slack: one for VISA and one for Jupyter development.*
- First workshop update
    - *WP3 and WP6 are interesting in attending the same workshop (Jamie)*
    - *Jakub mentioned that the details are still currently being finalised. The workshop will / should be held in Prague alongside the EOSC hub conference https://www.eosc-hub.eu/events/eosc-hub-week-2019*
- Hans' vision for Jupyter services (5 min + 10 min)
- XFEL Jupyter development demo (Robert Rosca, 10 min)
    - *Robert demonstrated using a Jupyter notebook for visalising Nexus data using the [Karabo framework](https://in.xfel.eu/readthedocs/docs/karabo/en/latest/concepts/introduction.html)*
    - *Robert will make this work public for the other partners*
    - *There was a discussion that Matplotlib is not designed for large datasets and we should start looking for a plotting engine for Jupyter to handle this.*
- First services to be put onto EOSC hub (Binder, Jupyter hub etc. 10 min)
    - *Deploy a binder instance onto EOSC hub*
- Confluence demo (Stuart and Jamie, 10 min)
  - *Not enough time to give the demo*
- AOB
    - *Eric sent an email to the mailing list about the hdf-viewer he has been working on:*
        - *https://code.ill.fr/panosc/data-analysis-services/hdf-viewer*
        - *https://pypi.org/project/hdfviewer/*
        - *https://hdf-viewer.readthedocs.io/en/latest/*
    - *Hans suggested creating a wiki page for links to projects / code / notebook examples  etc.*
        - *https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/resources/software.rst*
        - *https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/resources/jupyter-notebook-examples.rst*
    - Jamie suggested having a page with development tips and code guides e.g. 
        - *https://code.ill.fr/panosc/data-analysis-services/hdf-viewer/wikis/install-procedure-from-a-virtualenv-container*
