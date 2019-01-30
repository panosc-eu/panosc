# WP4 Meeting

**Date:** 29/01/2019

**Note:** Discussion and actions decided throughout the meeting are marked in italic

### Participants

- Jamie Hall (ILL)
- Stuart Caunt (ILL)
- Fabien Pinet (ILL)
- Kareem Galal (ESS)
- Jakub Grosz (ELI)
- Lottie Greenwood (ESS)
- Thomas Vincent (ESRF)
- Robert Rosca (XFEL)
- Jerome Kieffer (ESRF)

### Agenda

- **General organisation and feedback from the kick-off meeting**         
  - **Kick-off summary**
  - **Face-to-face meetings (how often? when? workshops? big conferences?)**
    - Decided during the kick-off meeting that we will have a video meeting every 2 weeks
      - Between WP4 leaders? Need to know who the WP4 leaders are at each institute. Unclear for the moment. Ideally, any one who is interested can join.
        - *WP4 leaders will let themselves be known*
        - *We have agreed that anyone can join the 2 weekly meetings*
        - *The meetings will be held at the same day and time*
    - Workshops every *n* months. ILL can offer to host the first workshop. ASAP ideally Mar/April to clearly define objectives and vision; much easier face-to-face
      - *Jakub (ELI) is currently organising a workshop for the end of march / beginning of April. He suggested we could have our first workshop there. Beginning of April would be ideal as hopefully most people will have been recruited by then. Discuss further with Jakub (ELI). If not at possible at ELI, ILL has suggested it can host the first workshop. The plans will be finalised before the end of February*
  - **Tools to use (slack, confluence, GitHub etc.)**
    - Slack
      - I'll be communicating more on slack, rather than the mailing lists
        - *People will contact Jamie (ILL) to be invited to slack*
        - *We are all open to the idea of using slack for quick discussions*
    - Mailing lists useful for more formal discussions, however, slack is better for quick discussions e.g. technical, developments, questions etc.
      - *All in agreement*
    - Feedback from WP1 meeting last week. EGI have offered to host a confluence instance for the PaNOSC project. Still waiting for confirmation from EGI for when this will happen
      - *Generally don't want to have documents all over the place but are open to checking out the advantages of confluence.*
    - ILL has setup a confluence instance internally. Would make external, however we don't have a license for the moment. Probably better to wait for EGI. It would be useful to use confluence for the WP4 docs, KPIs, risks, technical diagrams etc. But make do with what we have.
      - *Jamie (ILL) will discuss at the next management meeting about where we currently stand with EGI hosting a confluence instance*
    - There was discussion during the kick-off meeting for either me or Kareem (ESS) to present confluence
      - Is everyone still interested in that happening? When could we make that happen? At the next meeting?
      -  *Jamie (ILL) and Stuart (ILL) will give a short presentation at the next meeting*
    - Github
      - How do we organise projects on GitHub?
      - No possibility of subgroups on GitHub
      - Naming conflicts
      - Private repositories?
      - Any ideas?
    - Any other ideas?
      - *Still a bit vague*
      - *Ideally we would like one repository per development project*
      - *A naming convention could be useful to make it clear which project belongs to which work package (not prefixing with WP4 as it doesn't mean anything)*
      - *Jamie (ILL) will discuss this at the next management meeting*
  - **Licensing for new developments**
    - I've looked at licenses used throughout various European Projects. Not really much consensus.
    - Sent a message on slack
    - Thomas (ESRF) suggested using BSD-3 clause or MIT for Jupyter ecosystem
    - Tools developed outside of Jupyter, ILLs opinion is to use Apache License 2.0 for new developments
      - MIT is too open (not required to cite our work)
      - GPL is too restrictive
      - Any objections or opinions to using Apache License 2.0?
      - There are times where we won't be able to use the Apache License 2.0 due to the tools we're using
      - *Still unclear. Need a discuss with management. Thomas (ESRF) suggested to keep in line with the Jupyter ecosystem. ILL suggested Apache License 2.0. There was partial agreement that MIT could be too open - be good to cite the work. Need an official mandate from the management committee (Jamie(ILL) will contact them)*
  - **Survey of expertise and experience for each participating  institute (to be sent to each WP leader next week)**
    - Idea is to get a good idea of the expertise and experience at each institute for example, are most of the people working on WP4 developers, scientists or system administrators?
    - Will send a link to the survey
    - Need to identify WP4 institute leaders as discussed earlier
    - *Jamie (ILL) will send a questionniare at by the end of the week for each WP4 leaders to complete*
  - **Identify some key users (scientists) to follow the evolution of the WP at each institute**
    - Links to risks as will be discussed earlier
    - Need their expertise and feedback throughout the duration of the project
    - *Well received. All partners were in agreement. Action: identify at least three key users at each institute*
- **Technical work**         
  - **What are the immediate development goals?**
    - VISA
      - ILL will package VISA into an easy deployable solution for each institute to play around with.
        - *Action: to be packaged by ILL*
      - Could run a test instance on a cloud platform? OVH, DigitalOcean, AWS etc.
        - *Everyone was in agreement*
        - *Action: ILL to look into this*
      - Working group to define a specification for each institute e.g. use cases:
        - How do you access and mount data?
        - How do you authorise users?
        - How is your proposal system structure?
        - What Linux distribution do you use? Do you use Windows?
        - Should have input from each institute
        - Not linked to Task 4.1 (needs to be completed by M12 but we need this information ASAP)
        - *Well received. Each institute will participate in the working group. To be discussed at the next meeting of how to go ahead*
      - Jupyter
        - Discussed developing a HDF5 viewer at each institute
          - Duplicating work
          - *Kareem (ESS) suggested that reinventing the wheel is not the best idea. Be better to see on github what the other institutes have been working in order to gather ideas*
        - Find a use case for each institute and implement something (widget, viewer, reader etc.) inside Jupyter
          - ILL example: reading and writing ILL specific data format inside Jupyter
          - *Partners were open to the idea of finding a specific use case for their institute to implement into Jupyter*
          - *Action: to find a use case for each institute*
        - Working group
          - *Well received. Each institute will participate in the working group. To be discussed at the next meeting of how to go ahead*
        - Deploying a JupyterHub instance at each institute
          - *Agreed. Action: each institute will deploy a JupyterHub instance*
        - Could run a test instance on a cloud platform? OVH, DigitalOcean, AWS etc.
          - *Everyone was in agreement*
          - *Action: ILL to look into this*
        - More discussion with Hans is needed
  - **How is the work going to be distributed between the partners?**
    - Too early to say. Need feedback from institute survey 
    - Not everyone has been employed to start working on the project
    - *All agreed. Too early to distribute work. Will wait for the institute survey results*
  - **Data analysis requirements and solutions survey (task 4.1) discussion (google doc to crowd source ideas for the survey questions?)**
    - Send a google doc to crowd source ideas
      - *Jakub (ELI) suggested using a google survey instead of a google doc*
      - *Action: Jamie (ILL) will send a link to each everyone ASAP*
    - Technical needs, infrastructure, data analysis software, common workflows etc.
      - Discussion needs to be had between IT people and Scientists
        - *See above*
    - Would like this be finished by the end Feb/March so we have a clearer view for the path ahead.
      - *We agreed to have this finished by the end of March before the first workshop. This information is need ASAP as possible in order to better define objectives.*
  - **Who is available to start working right now?**
  - **Hiring update. Who will be starting on the project soon?  Open job positions etc.**
    - ILL is currently hiring. Looking to have new members on the team within 3 months
    - Anyone else currently hiring? Will they be starting soon?
      - *ESRF are currently recruiting*
      - *ELI are also recruiting*
      - *ESS are also recruiting (hopefully to have someone start in February)*
      - *ILL is currently recruiting two positions*
- **KPIs/Risk assessment**
  - KPIs
    - Send a google doc for KPIs ideas
      - *Everyone was in agreement. Action: Jamie (ILL) to send a document by the end of the week*
    - ILL has discussed a few KPIs:
      - Number of VMs used for data analysis
      - Number of active users taking advantage of VISA/Jupyter?
      - DOIs referencing analysis resources  / notebooks etc.
      - How much scientific software is available on both platforms?
  - Risk assessment
    - Not enough Risks outlined
    - Send a google doc for risk ideas
      - *Everyone was in agreement. Action: Jamie (ILL) to send a document by the end of the week*
    - ILL suggested that one risk could be that not many people will use the tools provided (high risk). This can be mitigated by getting some key users involved as discussed earlier.

- **AOB**

  - *Kareem talked about other people joining/taking over lead throughout the project and wondering if anyone could foresee any problems with that: nobody saw any problems*

- **Actions**

  - Identify and contact at least three keys users for each institute (All)

  - Deploy a JupyterLab instance at each institute

  - Complete the institute survey that will be sent at the end of the week (All)

  - Implement a use case into Jupyter for each institute (All)

  - Package VISA and remove ILL specific logic into an easily deployable package (ILL)

  - Analyse possibility of deploying VISA and JupyterLab onto a cloud instance (Jamie(ILL))

  - Create google docs for KPIs and Risks (Stuart(ILL)) and send to mailing list. Write down ideas for KPIs, Risks (All)

  - Create a google doc for Task 4.1 survey (Jamie (ILL)) and send to mailing list. Write down any questions (All)

  - Organise a confluence presentation (Jamie (ILL), Stuart(ILL))

  - Define working groups (Jupyter and Visa).  Create a google doc and people can add their names (Jamie (ILL))

    





