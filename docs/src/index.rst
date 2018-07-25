.. Permafrost Benchmark System documentation master file, created by
   sphinx-quickstart on Tue Jul 24 16:01:51 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Permafrost Benchmark System
===========================

:Release: |release|
:Date: |today|

The Permafrost Benchmark System (PBS) is **rad**!


pbs-executor
------------

The `PBS executor <https://github.com/permamodel/pbs-executor>`_
is deployed on a computational resource with ILAMB.
It provides two tools,
the `Model Ingest Tool`
for uploading CMIP5 model outputs,
and the `Benchmark Ingest Tool`
for uploading benchmark datasets.
These tools verify the uploaded files
and place them in the proper location
in the ILAMB directory tree.

.. toctree::
   :maxdepth: 3

   File module <pbs_executor.file>
   Ingest module <pbs_executor.ingest>
   Verify module <pbs_executor.verify>

   Basic Model Interface (BMI) <pbs_executor.bmi>


pbs-server
----------

.. toctree::
   :maxdepth: 2
   :caption: Contents:


Indices and tables
------------------

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
