.. Permafrost Benchmark System documentation master file, created by
   sphinx-quickstart on Fri Jul 27 08:35:06 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Permafrost Benchmark System
===========================

:Release: |release|
:Date: |today|

Getting Started Guide
---------------------

The **Permafrost Benchmark System** (PBS)
wraps the command-line
`ILAMB <https://bitbucket.org/ncollier/ilamb>`_
benchmarking software with a customized version of the
`CSDMS Web Modeling Tool
<https://csdms.colorado.edu/wiki/CSDMS_Web_Modeling_Tool>`_ (WMT),
and adds tools for uploading
`CMIP5-compatible <https://cmip.llnl.gov/cmip5/output_req.html>`_
model outputs and benchmark datasets.
The PBS allows users to access and run ILAMB remotely,
without having to install software or data locally;
a web browser on a desktop, laptop, or tablet computer
is all that’s needed.

.. toctree::
   :maxdepth: 1
   :caption: Contents:

   Registration <registration>
   Logging in to the PBS <login>
   The PBS Interface <layout>
   Using the ModelIngestTool <model-tool>
   Using the BenchmarkIngestTool <benchmark-tool>
   Saving a Tool <save-tool>
   Configuring an ILAMB Run <configure-ilamb>
   Running ILAMB <run-ilamb>
   Downloading Results <download-results>

The PBS project is supported by NASA grant NNX16AB19G,
*A Permafrost Benchmark System to Evaluate Permafrost Models*.
All content developed for this project is open source,
released under the Apache 2.0 license.
