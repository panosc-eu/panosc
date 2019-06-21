===============================
 Pansosc WP4 use cases at ESRF
===============================

In the scope of the work package 4 of Panosc, we propose to more particulary focus at ESRF on use cases based on the following data analysis softwares/situations:

- `PyNX <http://ftp.esrf.eu/pub/scisoft/PyNX/doc/>`_: Python tools for Nano-structures Xtallography
- `crispy <http://www.esrf.fr/computing/scientific/crispy/>`_: GUI to calculate core-level spectra using the semi-empirical multiplet approaches implemented in Quanty.
- `pyFAI <http://www.silx.org/doc/pyFAI/latest/>`_: Fast Azimuthal Integration using Python
- Processing using multiple nodes with GPUs such


PyNX
====

*PyNX* stands for Python tools for Nano-structures Xtallography.
It can be used for:

- Coherent X-ray imaging simulation and analysis:
  coherent diffraction imaging (CDI), Ptychography, Wavefront propagation, near field and far field techniques...
- Fast scattering calculations from large number of atoms and reciprocal space positions.

*PyNX* is fully optimised to use Graphical Processing Units, using either CUDA or OpenCL, to provide fast calculations with 1 to 3 orders of magnitude speedup compared to standard processor calculations.

- Documentation: http://ftp.esrf.eu/pub/scisoft/PyNX/doc/
- Source code: http://ftp.esrf.fr/pub/scisoft/PyNX/
- License: `CeCILL-B <http://www.cecill.info/licences/Licence_CeCILL-B_V1-en.html>`_ (French license similar to the FreeBSD license)


Use cases
---------

*PyNX* is usable either as command line scripts or through its Python API.
As such, in the scope of Panosc WP4 it is a use case for both remote desktop and jupyter notebooks.


Requirements
++++++++++++

- Single computer with Linux operating system and one GPU available for processing (through either OpenCL or CUDA).
- *PyNX* and dependencies installed (See http://ftp.esrf.fr/pub/scisoft/PyNX/doc/install.html).


Command line interface use case
+++++++++++++++++++++++++++++++

2D ptychography analysis example:

- Download the `ptycho-siemens-star-id01.cxi <http://ftp.esrf.fr/pub/scisoft/PyNX/data/ptycho-siemens-star-id01.cxi>`_ dataset:
  ``curl -O http://ftp.esrf.fr/pub/scisoft/PyNX/data/ptycho-siemens-star-id01.cxi``
- Run analysis script: ``pynx-cxipty.py data=ptycho-siemens-star-id01.cxi probe=focus,60e-6x200e-6,0.09 defocus=200e-6 algorithm=analysis,ML**100,DM**100,DM**100,nbprobe=3,probe=1 saveplot``
- Results are stored in the ``ResultsScan0000`` folder.
  The ``Run0001.cxi`` file (in HDF5 `CXI <https://www.cxidb.org/cxi.html>`_ format) contains the reconstructed sample (``entry_1/object/data``) and probe (``entry_1/probe/data``) stored as complex data images that can be visualized, e.g., with ``silx view``.

Additional information: `Readme <http://ftp.esrf.fr/pub/scisoft/PyNX/data/ptycho-siemens-star-id01-README.txt>`_


Notebook use case
+++++++++++++++++

- Sample notebooks (based on simulated data for now) are available here: http://ftp.esrf.fr/pub/scisoft/PyNX/example_notebooks/
- More notebooks available as part of the source distribution can be run on Binder: Go to the *PyNX* `binder environment <https://gitlab.esrf.fr/tvincent/PyNX-binder>`_ and press the launch button to start it on `mybinder <https://mybinder.org/>`_.
  Some notebooks might fail on `mybinder <https://mybinder.org/>`_ because they reach the memory limit or require a GPU.

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


pyFAI
=====

*pyFAI*: Fast Azimuthal Integration in Python.

*pyFAI* is an azimuthal integration library that tries to be fast (as fast as C and even more using OpenCL and GPU).
It is based on histogramming of the 2theta/Q positions of each (center of) pixel weighted by the intensity of each pixel, but parallel version uses a SparseMatrix-DenseVector multiplication.
Neighboring output bins get also a contribution of pixels next to the border thanks to pixel splitting.
Finally *pyFAI* provides also tools to calibrate the experimental setup using Debye-Scherrer rings of a reference compound.

- Documentation: http://www.silx.org/doc/pyFAI/latest/
- Source code: https://github.com/silx-kit/pyFAI
- License: `MIT <https://opensource.org/licenses/MIT>`_

Use cases
---------

*pyFAI* is a python library and thus in the scope of Panosc WP4 it is targeted for jupyter notebook usage.

Yet, it bundles a desktop GUI application based on PyQt.

Requirements
++++++++++++

- *pyFAI* runs on Linux, Windows and macOS.
  It can provide faster processing if a GPU is available for processing through OpenCL.
- *pyFAI* and dependencies installed (See http://www.silx.org/doc/pyFAI/latest/operations/index.html).

Azimuthal integration use case
++++++++++++++++++++++++++++++

- `Integration with Python cookbook <http://www.silx.org/doc/pyFAI/latest/usage/cookbook/integration_with_python.html>`_.
- *pyFAI* cookbook and tutorial notebooks can be run on Binder (The Binder environment description is integrated in the *pyFAI* source repository): |pyFAI myBinder Launcher|
  
  Note: Some notebooks fail on `mybinder <https://mybinder.org/>`_ because they reach the memory limit.

.. |pyFAI myBinder Launcher| image:: https://mybinder.org/badge_logo.svg
   :target: https://mybinder.org/v2/gh/silx-kit/pyFAI/master?filepath=binder%2Findex.ipynb

Calibration use case
++++++++++++++++++++

Performing the steps required to calibrate an experimental setup from a notebook.
This is currently available through a desktop GUI application (See http://www.silx.org/doc/pyFAI/latest/usage/cookbook/calib-gui/index.html).

This involves the following user interactions:

- drawing a bitmap mask on a detector image.
- selecting a few rings manually.


Processing on multiple nodes with GPUs
======================================

This a technical use case to assess the feasibility of running parrallel processing on multiple nodes of a compute cluster from a notebook for ,e.g., a tomography reconstruction.

- Source code: https://gitlab.esrf.fr/paleo/sidi
- License: `MIT <https://opensource.org/licenses/MIT>`_

Use cases
---------

This is a use case for jupyter notebooks.

Requirements
++++++++++++

- The notebook should be able to spawn jobs on a compute cluster.
- Dependencies: `distributed <http://distributed.dask.org/en/latest/>`_, `jobqueue <https://jobqueue.dask.org/en/latest/>`_

Use case
++++++++

- This notebook runs a filtered-backprojection to convert sinogram data to reconstructed slices using workers on a compute cluster: https://gitlab.esrf.fr/paleo/sidi/blob/master/examples/distributed_fbp.ipynb

