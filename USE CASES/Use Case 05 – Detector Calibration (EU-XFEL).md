Use Case 5 – Detector Calibration (European XFEL)
=========================================================

European XFEL uses a range of pixel detectors, including some which are custom built to cope with the high pulse rate. The raw data recorded from these detectors needs various corrections applied as a first step in analysing it.

The workflows for applying corrections and for creating the calibration constants they use are implemented in a collection of Jupyter notebooks.

Detector experts can conveniently work with a small amount of data to develop these notebooks interactively. A supporting software infrastructure runs the notebooks in parallel on the Maxwell cluster as new runs are saved, to create corrected data. The notebooks also generate plots and summary statistics to monitor the calibration quality, and the notebooks used for each run are converted into a PDF report saved alongside the data.

Developers:
------
M. Kuster, J.-S. Dambietz, S. Hauf, T. Kluyver, R. Rosca, Y. Kirienko

References:
------
[1] M. Kuster, D. Boukhelef, M. Donato, J.-S. Dambietz, S. Hauf, L. Maia, N. Raab, J. Szuba, M. Turcato, K. Wrona & C. Youngman (2014) Detectors and Calibration Concept for the European XFEL, Synchrotron Radiation News, 27:4, 35-38, DOI: 10.1080/08940886.2014.930809

[2] H. Fangohr, S. Brockhauser, et al. (2020) Data Exploration and Analysis with Jupyter Notebooks. Proc. ICALEPCS’19, 799—806. DOI:10.18429/JACoW-ICALEPCS2019-TUCPR02

PaNOSC related work packages:
------
[WP4 – Data Analysis Services](https://www.panosc.eu/work-packages/work-package-4-data-analysis-services/)

Contact person:
------
[Thomas Kluyver](mailto:thomas.kluyver@xfel.eu) (European XFEL)

More on PaNOSC github:
------
https://github.com/European-XFEL-examples/panosc-detector-calibration

LINK to website:
------
https://www.panosc.eu/use-cases/use-case-5-detector-calibration/
