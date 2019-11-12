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

