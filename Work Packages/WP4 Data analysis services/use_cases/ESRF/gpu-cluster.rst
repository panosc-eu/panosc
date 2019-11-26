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

