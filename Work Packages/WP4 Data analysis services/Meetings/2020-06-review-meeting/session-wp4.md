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
-   what will be demonstrate \[tidy up next sections\]
    -   portal
    -   reproducibility
    -   link to publications
    -   running simulaions, how could it be useful/very expensive
        beamtime
    -   interactive
    -   tool provision
        -   hdf5 integration into the web
        -   contribute to generic tools
-   sharing and linking with Expands

-   Summary: how does this help science today and in the future?
    -   facilities make it easier for users
    -   allows other scientists to take the work further
    -   how does this link with EOSC
    -   highlight shortcomings
        -   different scientific domains have different challenges
        -   ?

Context for each demo
---------------------

For all demonstrations, it is important to explain:

-   where is the demonstration executed? (local laptop/computer, remote
    compute facility, cloud compute)
-   where is the software / script coming from that is executed?
-   where is the data located that is used?
-   \[probably more\]

We should have a consistent way of showing this (ideally graphically).

2. Data portal, Jakup, \~10 mins
--------------------------------

key points to cover:

-   portal
-   finding data
-   application to lasers in example

Details:

-   showcase portal user interface and user experience
-   browse the data catalogue
-   basic filtering
-   select one example data set
-   particle in cell simulation
-   go to details page, then click on publication (?)
-   back to details page, launch notebook to modify parameter and update
    visualisation

3. Simulation, Thomas, \~10 mins
--------------------------------

key points to cover:

-   beam very expensive, produces lots of data (also expensive)
-   use simulation to prepare experiment, check feasibility, optimise
    experiment
-   across-facility example
-   explain quantities of data
-   can use simulation results to test and improve analysis processes

Details:

-   show simulation execution in notebook
-   show analysis of simulated experiment in notebook
-   if possible, run on EGI provided Binder (would be nice link to
    EOSC), alternatively Maxwell would be okay

4. Towards FAIR with Reproducible paper, Robert, 10 mins
--------------------------------------------------------

key points:

-   example starts from published results
-   compare figures from paper and re-computation
-   has been reproduced by somebody who is not an author with help of
    the author

\[- enables re-usability\]

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

key points:

-   example of scientist who produced reproducible analysis out of her
    own initiative, and published this on github
-   downloads data from ESRF catalogue

Details:

-   Describe the process (how many notebooks, and steps, ...)
-   show part of the process (one notebook, describe GUI interaction if
    required)
-   paper is nearly published
-   example for scientist pushing envelop of reporducibility -\>
    re-uability

6. Remote Desktop, could come from Franz (STFC/ExPaNDS), 10 mins
----------------------------------------------------------------

key points:

-   show case remote desktop as remote analysis technology
-   shows neutron example

Details:

-   neutrons and different remote analysis technology (?)

7. General purpose tools: HDF5 viewer, Axel, 10 mins
----------------------------------------------------

keypoints:

-   general purpose
-   reading data from HDF5 webserver
-   contribute to wider community (beyond Photon and Neutron Science)

Details:

-   introduce hdf5 briefly, and comment on wide spread use
-   HDF5 viewer demo
-   dissemination plans (open source)
-   show or report on (plans for) integration with JupyterLab
