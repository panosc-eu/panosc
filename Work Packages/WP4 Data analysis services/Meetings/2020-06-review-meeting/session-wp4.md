Presentation Work Package 4, draft
==================================

1. Introduction, Hans, \~10 mins
--------------------------------

-   WP4 motivation
    -   data analysis extracts meaning from data
    -   essential and non-trivial process in Photon and Neutron science
    -   reproducibility of the process from raw data to publication
    -   enables re-use and more effective science
-   WP4 objectives
    -   provide data analysis together with data
    -   control and execute data analysis remotely
    -   enable better reproducibility and re-usability
    
-   Details are in reports
-   Focus on demonstrations today
    -   data portal (slide with image)
    -   Jupyter Notebook and remote Desktop as remote analysis infrastructures
    -   Remote simulation to support experiments
    -   Link to publications & Reproducibility 
    -   sharing and linking with Expands
    -   tool provision
        -   HDF5 integration into the web
        -   contribute to generic tools
    
-   Summary: how does this help science today and in the future?
    -   facilities make it easier for users
    -   allows other scientists to take the work further
    -   how does this link with EOSC
    -   highlight shortcomings and challenges
        -   different scientific domains have different challenges
        -   data access
        -   central EOSC hosted portal 
            - architecture?
            

Context for each demo
---------------------

For all demonstrations, it is important to explain:

-   where is the demonstration executed? (local laptop/computer, remote
    compute facility, cloud compute)
-   where is the software / script coming from that is executed?
-   where is the data located that is used?
-   \[probably more\]

We should have a consistent way of showing this (ideally graphically).

2. Data portal, Jakub, \~10 mins
--------------------------------

Key points to cover:

-   portal
-   finding data
-   application to lasers in example

Details:

-   showcase portal user interface and user experience
-   browse the data catalog
-   basic filtering
-   select one example data set
-   particle in cell simulation
-   go to details page, then click on publication (?)
-   back to details page, launch notebook to modify parameter and update
    visualisation

3. Simulation, Thomas, \~10 mins
--------------------------------

Key points to cover:

-   beam very expensive, produces lots of data (also expensive)
-   use simulation to prepare experiment, check feasibility, optimise
    experiment
-   across-facility example
-   explain quantities of data
-   can use simulation results to test and improve analysis processes
-   Example for Jupyter Notebook driven computation and analysis

Details:

-   show simulation execution in notebook
-   show analysis of simulated experiment in notebook
-   if possible, run on EGI provided Binder (would be nice link to
    EOSC), alternatively Maxwell would be okay

4. Towards FAIR with Reproducible paper, Robert, 10 mins
--------------------------------------------------------

Key points:

-   example starts from published results
-   compare figures from paper and re-computation
-   has been reproduced by somebody who is not an author with help of
    the author
-   enables re-usability
-   Jupyter Notebook example
-   improvement: if created at publication time, can create extra DOI
    for analysis

Details:

-   provide a little context for paper
-   show paper and figures in it
-   execute re-production of paper (on EGI binder?)
-   compare reproduced figures with published figures
-   comment on data situation: data set so small that it is embedded
    with software

5. User provided reproducible publication, Thomas V, 10 mins
------------------------------------------------------------

Key points:

-   example of scientist who produced reproducible analysis out of her
    own initiative, and published this on GitHub
-   downloads data from ESRF catalog
-   Jupyter Notebook and GUI example

Details:

-   Describe the process (how many notebooks, and steps, ...)
-   show part of the process (one notebook, describe GUI interaction if
    required)
-   paper is nearly published
-   example for scientist pushing envelop of reproducibility -\>
    re-usability

6. Remote Desktop, could come from Franz (STFC/ExPaNDS), 10 mins
----------------------------------------------------------------

Key points:

-   show case remote desktop as remote analysis technology
-   shows neutron example

Details:

-   neutrons and different remote analysis technology (?)

7. General purpose tools: HDF5 viewer, Axel, 10 mins
----------------------------------------------------

Key points:

-   general purpose
-   reading data from HDF5 web server
-   contribute to wider community (beyond Photon and Neutron Science)

Details:

-   introduce HDF5 briefly, and comment on wide spread use
-   HDF5 viewer demo
-   dissemination plans (open source)
-   show or report on (plans for) integration with JupyterLab



Overall timings
---------------

- assume 90 minute slot in total
- currently 7 presentations -> 20 minutes spare
  - 2 additional minutes questions per presentation, so we can fill a 90 minute slot.
