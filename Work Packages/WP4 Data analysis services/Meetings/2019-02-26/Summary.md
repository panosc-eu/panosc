## WP4 meeting - 26/02/2019

## Participants

Jamie (ILL), Stuart (ILL), Fabien (ILL), Eric (ILL), Hans (XFEL), Robert (XFEL), Enol (EGI), Jakub (ELI), Lottie (ESS), Aidan (ESRF), Thomas (ESRF), Ornela (CERIC-ERIC), Andy (ESRF)

## Agenda

- Hiring updates

- - *EuXFEL: 1 person hired for WP4 (Robert Rosca), complete for now*
  - *ILL - interviews next week for software developer. 2 positions still being confirmed.*
  - *ESS have offered a contract to someone (working on WP3 and WP4)*
  - *ESRF is recruiting someone that will be working mostly on administrative tasks. A position for recruiting a developer is currently in progress.*
  - CERIC-ERIC - ?
  - *ELI - Recruiting for two positions (one for WP4 and one for WP3)*

- Documents on github for software we work on (WP4):

- - <https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/resources/software.rst>

- Documents on github for jupyter notebook examples:

- - <https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/resources/jupyter-notebook-examples.rst>

- EGI notebooks (EGI) 

- - [*notebooks.egi.eu*	](http://notebooks.egi.eu)
  - *A few of us have tried it*
  - *We will send our feedback / comments to Enol (EGI)*

- Institute feedback results

- - *Jamie (ILL) has sent the results to the WP4 members*

- Summary from FTS3 WP6 meeting

- - *Slides and minutes from the meeting are up on github:*

  - - [*https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP6%20EOSC%20Integration/WP6%20Telco%20%232.md*](https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP6%20EOSC%20Integration/WP6%20Telco%20%232.md)
    - [*https://github.com/panosc-eu/panosc/raw/master/Work%20Packages/WP6%20EOSC%20Integration/PANOSC_Presentation.pptx*](https://github.com/panosc-eu/panosc/raw/master/Work%20Packages/WP6%20EOSC%20Integration/PANOSC_Presentation.pptx)
    - *Hans (XFEL) mentioned that one of the first services that should be put up onto EOSC hub is a binder service.* 

- Workshops 

- - *Jupyter dashboarding details in Paris:*

  - - [*https://blog.jupyter.org/jupyter-community-workshop-dashboarding-with-project-jupyter-b0e421bdf164*](https://blog.jupyter.org/jupyter-community-workshop-dashboarding-with-project-jupyter-b0e421bdf164)
    - *Dates: June 3rd to June 6th*
    - *Planned attendance from WP4: Robert Rosca (EuXFEL),  Eric (ILL),  ... ?*

  - EGI event in Amsterdam (EGI organised, plan for Jupyter dedicated session)

  - - *Jakub (ELI)  proposed we could spend 1 - 1.5 days doing a workshop for WP4. Hans (XFEL) suggested that we should extend this as we would probably need more time to discuss.*
    - *Dates: 6-8 May 2019*
    - [*https://www.egi.eu/news/registration-for-the-egi-conference-2019-is-now-open/*](https://www.egi.eu/news/registration-for-the-egi-conference-2019-is-now-open/)
    - *Planned attendance from WP4:* ?

  - *EOSC hub event:*

  - - [*https://www.eosc-hub.eu/events/eosc-hub-week-2019*](https://www.eosc-hub.eu/events/eosc-hub-week-2019)
    - *Dates: 10 - 12 April 2019*

- Task 4.1 survey. Can we get it finalised before the next meeting?

- - *We agreed that it we would get this finalised before the next meeting*
  - *Andy (ESRF) sent us a survey that was done for the Calipsoplus project:* [*http://www.calipsoplus.eu/wp-content/uploads/2018/09/D24-3_reported.pdf*](http://www.calipsoplus.eu/wp-content/uploads/2018/09/D24-3_reported.pdf)

- We need to get uses cases and scientists involvement ASAP.

- - *Robert (XFEL) mentioned that he is currently working with one of the scientists at XFEL and that he is following the WP.*
  - *Jamie (ILL) mentioned that the ILL is still currently finalising details for finding a group of scientists.*

- HDF viewer demo

- - *Thomas mentioned that one putative source of the problem for the browser that freezes when using the matplotlib cursor could be that there is a continuous rendering from the ipython kernel which triggers never ending connection from ipython to jupyter-lab frontend.* 

  - *Eric proposed that the prototype should be test around the wp4 team especially to check how it scales for big datasets.*

  - *We agreed that other plotting packages should be investigated (e.g. bqplot).*

  - *When discussing about the importance of adding “true” 3D view of the data, Hans mentioned that the current 2D slice view proposed in the prototype may be sufficient for investigating 3D datasets.*

  - *Hans mentioned two technologies for 3d interactive graphics in the notebook:* 

  - - *K3d (*[*https://github.com/K3D-tools/K3D-jupyter/blob/master/README.md*](https://github.com/K3D-tools/K3D-jupyter/blob/master/README.md)*)*
    - *Ipyvolume* [*https://ipyvolume.readthedocs.io/en/latest/*](https://ipyvolume.readthedocs.io/en/latest/) 	

- AOB

## Actions

1. Everyone should look at the Task 4.1 survey and offer their input before finalising it for the next meeting.
2. Identify at least one use cases at each facility (requests for more to follow)