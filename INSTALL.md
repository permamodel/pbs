# Installing the PBS

The PBS uses a customized instance
of the [CSDMS Web Modeling Tool](https://csdms.colorado.edu/wiki/CSDMS_Web_Modeling_Tool) (WMT).
For help in setting up WMT and installing the PBS,
it's recommended that you please
[contact](csdmssupport@colorado.edu) the developers.
However,
if you're keen to try this on your own,
some notes follow.
Be aware that WMT requires a substantial amount of manual configuration.

WMT is comprised of three components:

* *executor* = the computational resource, ranging from a beefy
  desktop to a supercomputer, on which jobs are run
* *server* = the web backend which stores and submits jobs and serves
  outputs
* *client* = the web UI

Each of these components has a separate installation,
possibly on separate machines.
The PBS has components that augment each of these installations.


## Executor

The [ILAMB](https://bitbucket.org/ncollier/ilamb) benchmarking system
forms the core of the PBS.
It has install instructions,
including dependencies,
in its [documentation](https://ilamb.ornl.gov/doc/).
WMT requires the
[wmt-exe](https://github.com/csdms/wmt-exe),
[pymt](https://github.com/csdms/pymt), and
[babelizer](https://github.com/bmi-forum/babelizer) packages.
PBS requires the
[pbs-executor](https://github.com/permamodel/pbs-executor) and
[bmi-ilamb](https://github.com/permamodel/bmi-ilamb) packages.
Some notes on setting up a PBS executor are given
[here](https://csdms.colorado.edu/wiki/PbsExecutorSiwenna).
A restricted user,
with read-write access to the ILAMB files,
should be created for use with the PBS.


## Server

On the server,
WMT requires the
[wmt](https://github.com/csdms/wmt) and
[wmt-metadata](https://github.com/csdms/wmt-metadata) packages.
PBS requires the
[pbs-server](https://github.com/permamodel/pbs-server) package.
Some notes on setting up a PBS executor are given
[here](https://csdms.colorado.edu/wiki/PbsServerDiluvium).


## Client

The
[wmt-client](https://github.com/csdms/wmt-metadata)
should be installed on the server
using the `reference/pbs` branch.
