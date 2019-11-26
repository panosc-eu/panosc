crispy
======

*crispy* is a modern graphical user interface to calculate core-level spectra using the semi-empirical multiplet approaches implemented in `Quanty <http://quanty.org/>`_.
The interface provides a set of tools to generate input files, submit calculations, and plot the resulting spectra.

- Documentation: http://www.esrf.fr/computing/scientific/crispy/
- Source code: https://github.com/mretegan/crispy
- License: `MIT <https://opensource.org/licenses/MIT>`_

Use case
--------

*crispy* is a desktop GUI application based on PyQt.
In the scope of Panosc WP4 it should be used through remote desktop access.


Requirements
++++++++++++

- *crispy* runs on Linux, Windows and macOS.
- *crispy* and dependencies installed (see http://www.esrf.fr/computing/scientific/crispy/installation.html)

Use case
++++++++

Calculating the L-edge X-ray absoption spectrum of nickel compounds:

- Open the application.
- Change the Gaussian broadening to 0.3 eV; press Return after entering the new value.
- Press the Run button to start the calculation.
- After the calculation finishes, the spectrum will be automatically plotted.

Additional information: `see the tutorial <http://www.esrf.fr/computing/scientific/crispy/tutorials/ni_ligand_field.html>`_

