Use Case 19 – Online visualization and analysis of Bruker NMR output
=========================================================	
Nuclear Magnetic Resonance (NMR) spectroscopy is a technique widely used in characterization of various chemical compounds, providing information about the atomic electronic structure of molecules. [Bruker](https://www.bruker.com/en/products-and-solutions/mr.html) is a world leader in the sector of NMR spectrometers. Bruker NMR devices output raw data in a proprietary format, that is processed by both open source and proprietary software, such as nmrpipe, and visualized through tools such as [nmrdraw](https://nmr.chem.ucsb.edu/protocols/nmrPipe.html) and Sparky. Installation of these tools is demanding, and requires training. Users use boilerplate code for their needs and have to switch between different tools to achieve an optimal calibration. The difference between spectrometers (while using the same code) can lead to a reduced reproducibility, and a general difficulty in sharing data, or performing analysis for remote users.

We have designed and developed an easy-to-use online solution for treatment of Bruker NMR files, FidViewer (allowing other formats as well). It replaces a number of aforementioned programs and provides for a transparent and efficient workflow, focusing the user on scientific content rather than the software itself.

FidViewer solves the issues by providing an interactive web tool where users can upload different formats of Bruker NMR data (FID, FT2, or ZIP files with the raw acquisition data folders), to visualize already processed data or perform phase shift calibration, visualizing countour plots to identify peaks, and marginal plots to visualize sections of the dataset on specific coordinates.

Main Contributors
------
* Andrea Lorenzon ([CERIC-ERIC](https://www.ceric-eric.eu/)) – Software engineering, developer, design
* [Peter Podbevšek (Slovenian NMR Centre)](http://www.slonmr.si/personnel/peter_podbevsek.php) – Design, validation, testing

Use Case Action Flow
------
* Loading: Load Bruker FID, FT2 and Zip files with raw data folders.
* Visualisation: Create real time tunable contour plot for the data matrix.
* Marginals plots: Visualize, for specific coordinates, marginal plots with a section of the data matrix.
* Analysis: Option to process data, applying a standard pipeline, with the ability of manually tune phase shift parameters.
* Export: Export and download processed data in FT2 format for further analytics and sharing.

Description of needs
------
The service will be integrated into the CERIC-ERIC EOSC service portfolio. FidViewer will progressively fit more in the PaNOSC universe, and as soon as other tools are ready, integrated with them: e.g., the Search API and Data Catalog will replace or integrate the file upload tool.

Impacts from the implementation
------
Remote users can visualize and analyse NMR data without the need to install software. Fast online tuning and conversion, with immediate visual feedback, save a lot of time currently needed to switch between processing and visualization tools. The workflow thus becomes more transparent and reproducible.

Generalisation of the use case
------
Any Bruker NMR user can benefit from this tool, both in academia and industry. Furthermore, an API can be developed for any NMR spectrometer.

Resources
------
The application is a python Streamlit standalone app, with a backend that is based on numpy, nmrglue, and matplotlib.

Code and documentation can be found at https://gitlab.elettra.eu/panosc/fidviewer

PaNOSC-related work package
------
[WP4 – Data Analysis Services](https://www.panosc.eu/work-packages/work-package-4-data-analysis-services/)

Contact person
------
[Andrea Lorenzon](mailto:andrea.lorenzon@ceric-eric.eu) (CERIC-ERIC)
