Use Case 23 – BRAGGY diffraction image viewer
=========================================================
In the context of remote operation, there is a need to create an application for browsing and visualising diffraction data, so that the users of the [ESRF MX beamlines](https://www.esrf.fr/UsersAndScience/Experiments/MX/About_our_beamlines) can easily view the data they acquire. At present, the data is stored in either HDF5 or CBF files produced by Pilatus, Eiger and Jungfrau detectors.

The detectors are controlled through the same software (LIMA, and eventually LIMA v2) and it can therefore be assumed that the CBF header or HDF5 metadata format is consistent. HDF5 files are further expected to comply with the NEXUS format.

The long-term goal of the application would be to extend the application to not only display diffraction data, but also other kinds of data stored in HDF5 format.

The application backend will be developed as a web application by merging existing features of Braggy with a Daiquiri backend. A new custom frontend will be created by reusing parts of the Braggy frontend with UI components from the H5Web library.

The application is to be used alongside with the MXCuBE beamline control application and performance, and bandwidth consumption should be carefully evaluated.

The project will mainly focus on the basic use cases, to develop a prototype so that the performance and user experience can be assessed. Refinements, as well as the extra use cases will then be implemented in a second phase.

Main Contributors
------
* **Marcus Oscarsson** – Requestor of use case, developer of MxCube web application, will integrate Braggy into MxCube and coordinate tests with scientists.
* **Axel Bocciarelli** – PaNOSC developer of h5web web UI, will extend h5web for Braggy.
* **Loic Huder** – PaNOSC developer of h5web web tools and backend h5grove, will integrate extend h5grove and h5web for Braggy.

Use Case Action Flow
------
* Browsing + Viewing: A user can ONLY browse and display HDF5 and CBF data located in the shift attributed data folder /data/…./mx[abc123]
* Display metadata: The user should be able to visualize information derived from the header or metadata, such as resolution, energy, angles, and so on.
* Zooming: The user should be able to change the colour map and scaling the data (including min/max values), zoom in the frame and display values of the pixels. The user should be able to zoom and display values of the pixels.
* Security: Limit the access to the data, so that only the user(s) that are owners of the data can access it.

Description of needs
------
Implement a web-based image viewer adapted to diffraction images from macromolecular crystallography experiments (MX) specifically.

Impacts from the implementation
------
Scientists doing MX experiments remotely will be able to browse and view their data via the web. The PaNOSC h5web will be used as the basic building brick.

Generalisation of the use case
------
Braggy is potentially useful for all sites using the web-based version of MxCubeV3 for their remote experiments. These include MAX IV Laboratory and SOLEIL Synchrotron. It could be useful for other types of diffraction experiments as a web-based viewer for images.

Future developments of interest are:

The possibility for some limited ways to control the viewer remotely, i.e. from MXCuBE move to the directory where they are currently collecting data.
* To be able to automatically follow images from one location.
* To be able to play a sequence of images as a movie.
* To be able to visualise the intensity of a line and area cross section.
* To be able to perform frame summation.

Other partners interested in this use case
------
* [MAX IV Laboratory](https://www.maxiv.lu.se/)
* [Synchrotron SOLEIL](https://www.synchrotron-soleil.fr/en)

Resources
------
* [H5web](https://github.com/silx-kit/h5web)
* [H5web-braggy](https://gitlab.esrf.fr/ui/h5web-braggy)

PaNOSC related work packages
------
* [WP3 – Data catalogue services](https://www.panosc.eu/work-packages/work-package-3-data-catalog-services/): Data repository and search API
* [WP4 – Data analysis services](https://www.panosc.eu/work-packages/work-package-4-data-analysis-services/): Web interface to data portal
* [WP6 – EOSC integration](https://www.panosc.eu/work-packages/work-package-6-eosc-integration/): Download service

Contact person
------
[Andy Götz](mailto:andy.gotz@esrf.fr) (ESRF)
