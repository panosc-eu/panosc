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

