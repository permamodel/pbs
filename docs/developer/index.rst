.. Permafrost Benchmark System documentation master file, created by
   sphinx-quickstart on Tue Jul 24 16:01:51 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Permafrost Benchmark System
===========================

:Release: |release|
:Date: |today|

Developer Guide
---------------

The **Permafrost Benchmark System** (PBS)
is a customized version of the
`CSDMS Web Modeling Tool
<https://csdms.colorado.edu/wiki/CSDMS_Web_Modeling_Tool>`_ (WMT).
It wraps the command-line-driven
`ILAMB <https://bitbucket.org/ncollier/ilamb>`_
benchmarking software with a web interface,
and includes tools for uploading
`CMIP5-compatible <https://cmip.llnl.gov/cmip5/output_req.html>`_
model outputs and benchmark datasets.
The PBS allows users to access and run ILAMB remotely,
without having to install software or data locally;
a web browser on a desktop, laptop, or tablet computer
is all that's needed.

The source code described in this developer documentation
is available at https://github.com/permamodel/pbs.
The PBS developers welcome input from the community.
Feel free to submit an issue,
or fork any of the repositories that comprise the PBS,
modify them, and send us a pull request.


pbs-executor
------------

The `PBS executor <https://github.com/permamodel/pbs-executor>`_
is deployed on a computational resource alonside
`ILAMB <https://bitbucket.org/ncollier/ilamb>`_.
It provides two tools,
the `Model Ingest Tool`
for uploading CMIP5 model outputs,
and the `Benchmark Ingest Tool`
for uploading benchmark datasets.
These tools verify uploaded files
and place them in the proper location
in the ILAMB directory tree.

.. toctree::
   :maxdepth: 3

   File module (executor) <pbs_executor.file>
   Ingest module <pbs_executor.ingest>
   Verify module <pbs_executor.verify>
   Basic Model Interface (PBS) <pbs_executor.bmi>


pbs-server
----------

The `PBS server <https://github.com/permamodel/pbs-server>`_
is deployed on a
`WMT <https://csdms.colorado.edu/wiki/CSDMS_Web_Modeling_Tool>`_ server.
It constructs the configuration file used by
`ILAMB <https://bitbucket.org/ncollier/ilamb>`_,
and it handles any modifications to ILAMB metadata
resulting from users uploading model outputs
or benchmark datasets through the PBS.

.. toctree::
   :maxdepth: 2

   File module (server) <pbs_server.file>
   Models module <pbs_server.models>
   Variables module <pbs_server.variables>


bmi-ilamb
---------

The `bmi-ilamb <https://github.com/permamodel/bmi-ilamb>`_
package wraps `ILAMB <https://bitbucket.org/ncollier/ilamb>`_
in a `Basic Model Interface <http://bmi-spec.readthedocs.io>`_,
allowing ILAMB and the PBS tools to communicate.

.. toctree::
   :maxdepth: 2

   Config module <bmi_ilamb.config>
   Basic Model Interface (ILAMB) <bmi_ilamb.bmi>


Indices and tables
------------------

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
