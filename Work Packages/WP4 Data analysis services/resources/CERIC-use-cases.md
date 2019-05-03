# PaNOSC WP4 use cases at CERIC

## CERIC plans at a glance
[CERIC](https://www.ceric-eric.eu/about-us/who-we-are/) is an European Research Infrastructure Consortium (ERIC) with 8 partners facilities:

* [Graz University of Technology](https://www.ac.tugraz.at/index.php/wbPage/wbShow/aboutus?lang=en) (Austria)
* [Ruđer Bošković Institute](https://www.irb.hr/eng) (Croatia)
* [Charles University Prague](https://physics.mff.cuni.cz/kfpp/povrchy/?jaz_id=2&do=setLang) (Czech Republic)
* [Hungarian Academy of Sciences – Centre for Energy Research](http://www.bnc.hu/) (Hungary)
* [Elettra Sincrotrone Trieste](http://www.elettra.trieste.it/) (Italy)
* [Polish Ministry of Science and Higher Education](http://www.synchrotron.uj.edu.pl/en_GB/start) (Poland)
* [National Institute of Material Physics](http://lab50.infim.ro/) (Romania)
* [National Institute of Chemistry](https://www.ki.si/en/) (Slovenia) 

As it has instruments and [labs](https://www.ceric-eric.eu/users/labs-and-instruments/) placed over them, we plan to focus on implementations of remote services for CERIC’s beamlines placed at Elettra as a starting point. 

Elettra has a web portal called [VUO](https://vuo.elettra.eu) (Virtual Unified Office) that already allows for remote access of experimental data to users and scientists. We are currently working in an integration of data analysis services (e.g., [a web based HDF5 viewer](https://github.com/ElettraSciComp/h5nuvola), Jupyter based data analysis) to the existing portal. The VUO system is currently being developed in partnership with CERIC aiming at integrating other CERIC facilities to the portal. This could be a solution for us as a portal for data analysis services.

We propose the following data analysis softwares as use cases at CERIC:

* [VUO](https://vuo.elettra.eu) + [h5nuvola](https://github.com/ElettraSciComp/h5nuvola) (web based HDF5 viewer): Integration of existing facility portal to web-based data analysis services.
* [PyMca](http://pymca.sourceforge.net/): X-ray Fluorescence Toolkit.

## VUO + h5nuvola

VUO stands for Virtual Unified Office. It is mainly used for:
* Management of the whole lifecycle of an experiment (proposal submission, access to experimental data results, publication of results)
* Allows for remote access to the data storage

h5nuvola is a web-based data visualisation application equivalent for HDFView. Its main features are:
* Cloud file browsing
* Data visualisation services
* Exporting of data

### Software:

* Documentation: https://github.com/ElettraSciComp/h5nuvola
* Source code: TBD
* License: [GPL-v3](https://www.gnu.org/licenses/gpl.html)

### Use cases

The integration of the facility's web portal to a web-based data analysis services would allow beamline scientists and users to visualise experimental data through the web.

Integration to JupyterHub would fit with WP4 goals.


## PyMca

PyMca implements most of the needs of X-ray fluorescence data analysis. It can be used for fitting X-ray powder diffraction (XRD) data usually stored in HDF5 files.

### Software

* Documentation: http://www.silx.org/doc/PyMca/latest/tutorials.html
* Source code: https://sourceforge.net/projects/pymca/
* License: [MIT](https://opensource.org/licenses/MIT)

### CLI use case

TBD

### GUI use case 

A graphical user interface is available and is useful for certain data analysis tools like multichannel analyser (MCA), RGB correlator and image processing resources. It could be used through remote desktop access in PaNOSC WP4 context.
