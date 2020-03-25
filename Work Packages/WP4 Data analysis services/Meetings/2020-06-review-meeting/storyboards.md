# Drafts of potential presentations (live demos) for review meeting

Instructions at https://github.com/panosc-eu/panosc/blob/master/Work%20Packages/WP4%20Data%20analysis%20services/Meetings/2020-02-25/notes.org#actions

# EuXFEL Suggestions

## Reusing X-ray Gas Monitor Paper Results

### Scenario

Scientist reads a paper: https://doi.org/10.1107/S1600577519003795

They have an idea while reading the paper about some potentially interesting phenomena, which should be visible in the data.

The journal page has a link to the archived analysis on the PaNOSC portal, the scientist clicks the link, logs in with their university credentials, has access to the data as well as the notebooks used to create the results in the paper.

They can work on the results and expand on the analysis, save their work, and then share it with others.

## Presentation

Scenario based on: https://mybinder.org/v2/gh/European-XFEL-examples/jsr-operation-xgm-euxfel-paper/dev?filepath=notebooks%2Freadme.ipynb

Take a screenshot of the journal page, add in a link to "our portal".

Show mockup of our portal with SSO page using Umbrella, where the scientist selects his university and logs in with uni credentials.

The notebook starts up a page in a similar way to binder (add in some PaNOSC branding to mockup).

Scientist finishes work, closes notebook, and has the option to get a shareable link.

Final slide is scientist sending the link to a colleague.


## New Analysis Example

### Scenario

Scientist wants to explore some data.

Goes to PaNOSC portal, searches for the type of data they are interested in. The unified metadata catalogue between facilities shows all the matching results regardless of where the data was taken or where it is stored.

The scientist selects the data they want to analyse, decides to start up a notebook, and does their work.

They then save the notebook (and associated environment), and get an option to share it to others.

### Presentation

Start with some realistic example of analysis a scientist would like to do.

Explain/show how they might struggle to find the data they need, and then struggle to get access to it, and then to download it to their facility.

Then show mockups of the PaNOSC search function, and how it has results form all partner facilities. Also show a mix of results, maybe both experimental and simulated.

Show mockup of save and share dialogue. Explain how usually sharing your code can be difficult due to problems with fully specifying what dependencies your code has, and what versions, etc...

Final slide can be somebody else starting up the scientists analysis to build on top of it, concluding by saying this facilitates collaboration.

Try to slip FAIR points onto slides where relevant.

## Simulated Serial Crystallography

### Scenarios

New researchers want to get hands-on experience of data processing for
serial crystallography. Starting from a working example of a simulation coupled
to an analysis pipeline, they can explore how different experimental conditions
and different analysis options affect the results. For instance, they could
estimate how much data is needed in a given experimental setup.

Research software engineers working on serial crystallography analysis and
simulation want to test new software methods. By replacing either component of
a working example, they can compare the quality and performance of new
developments against a baseline.

### Presentation

- Overview of serial crystallography: diffraction patterns from individual,
  randomly oriented crystals.
- Challenge of turning diffraction patterns into 3D molecular structure
- Introduce simulation: a way to validate methods
- Show a few simulated detector images (compare to real images?)
- Illustrate getting from simulated images to (at least) unit cell parameter
  histograms as first scientific result.
  - Probably relies on "here's one I prepared earlier" to handle necessary data
    volume
- Show how easily we can change simulation/analysis parameters and re-run.
- Simulation examples don't have to run where the data is - can we automatically
  pick a facility to run it where load is low.
