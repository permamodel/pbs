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
<https://csdms.colorado.edu/wiki/Tools_portal#WMT>`_ (WMT),
and adds tools for uploading
`CMIP5-compatible <https://cmip.llnl.gov/cmip5/output_req.html>`_
model outputs and benchmark datasets.
The PBS allows users to access and run ILAMB remotely,
without having to install software or data locally;
a web browser on a desktop, laptop, or tablet computer
is all that’s needed.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   Registration <registration>
   Logging in to the PBS <login>
   The Layout of the PBS Interface <layout>
   Using the ModelIngestTool <model-tool>
   Using the BenchmarkIngestTool <benchmark-tool>
   Configuring an ILAMB Run <configure-ilamb>
   Running ILAMB <run-ilamb>
   Downloading Results <download-results>


Indices and tables
------------------

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
