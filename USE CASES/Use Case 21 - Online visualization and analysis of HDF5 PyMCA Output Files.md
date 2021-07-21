USE CASES/Use Case 21 - Use Case 21 - Online visualization and analysis of HDF5 PyMCA Output Files
=========================================================
X-Ray Fluorescence (XRF) is a non-destructive analytical technique used to determine the elemental composition of materials. XRF analysers determine the chemistry of a sample by measuring the X-ray photons emitted from a sample when it is excited by a primary X-ray source. Each of the elements present in a sample produces a set of characteristic emitted X-rays (“a fingerprint”) that is unique for that specific element, which is why XRF spectroscopy is an excellent tool for qualitative and quantitative analysis of material composition.

One of the best available tool to process XRF spectra is [PyMCA](http://pymca.sourceforge.net/), a ready to use, and in many aspects state-of-the-art, set of applications implementing most of the needs of X-ray fluorescence data analysis. It runs under Windows or MacOS. It can be run also as Python module.

PyMCA uses HDF5 as an open format to export data and metadata.

With this use case we aim to provide a stateless web app where users can upload a PyMCA HDF5 output, explore it, envision datasets and their content both as raw data matrices and as plots, customize every plot aspects, and perform transformations on included data, like log-transforms, missing data imputation, combination of different matrices (basic operation and evaluation of advanced matrix expressions).

Main Contributors
------
* **Alessandra Gianoncelli** ([ELETTRA](https://www.elettra.trieste.it/it/index.html)) Design, validation, testing
* **George Kourousias** ([ELETTRA](https://www.elettra.trieste.it/it/index.html)) Original concept, initial specifications, design
* **Andrea Lorenzon** ([CERIC-ERIC](https://www.ceric-eric.eu/)) Software engineering, developer, design

Use Case Action Flow
------
* Loading: Load XRF PyMCA experimental results in HDF5 format
* Visualisation: Create real time tunable plots for the data matrix
* Analysis: Option to process already fitted data, applying different transformations, and customize plot parameters

Description of needs
------
The service will be integrated into the CERIC-ERIC EOSC service portfolio. XrfFitVis will progressively fit more in the PaNOSC universe, and as soon as other tools are ready, integrated with them: e.g., the Search API and Data Catalog will replace or integrate the file upload tool.

Impacts from the implementation
------
Remote users can visualize and analyse PyMCA data without the need to install software. Users will be able to share data and perform repeatable remote analysis. The workflow thus becomes more transparent and reproducible. Users will also be able to perform computation on single or multiple data matrices, combining them both with a simple user interface, or with more advanced numpy-like syntax.

Generalisation of use case
------
Any PyMCA NMR user can benefit from this tool, both in academia and industry.

Partners
------
SRF is the main developer of PyMCA and implicitly included as stakeholder in this use case. Any facility involved in X-Ray Fluorescence experiments that are actually using PyMCA will be able to benefit from XrfFitVis.

Resources
------
The application is a python Streamlit standalone app, with a backend that is based on h5py, numpy, and matplotlib.

Code and documentation can be found at https://gitlab.elettra.eu/panosc/xrffitvis/

Other resources: https://xrffitvis.elettra.cs.ceric-eric.eu/

Contact person
------
[Andrea Lorenzon](mailto:andrea.lorenzon@ceric-eric.eu) (CERIC-ERIC)
