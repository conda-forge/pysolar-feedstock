About pysolar-feedstock
=======================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/pysolar-feedstock/blob/main/LICENSE.txt)

Home: http://pysolar.org/

Package license: GPL-3.0

Summary: A collection of Python libraries for simulating the irradiation of any point on earth by the sun

Development: https://github.com/pingswept/pysolar

Documentation: http://docs.pysolar.org/en/latest/

Pysolar is a collection of Python libraries for simulating the irradiation of any point on earth by the sun.
It includes code for extremely precise ephemeris calculations, and more.


Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=3247&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/pysolar-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-pysolar-green.svg)](https://anaconda.org/conda-forge/pysolar) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/pysolar.svg)](https://anaconda.org/conda-forge/pysolar) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pysolar.svg)](https://anaconda.org/conda-forge/pysolar) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/pysolar.svg)](https://anaconda.org/conda-forge/pysolar) |

Installing pysolar
==================

Installing `pysolar` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `pysolar` can be installed with `conda`:

```
conda install pysolar
```

or with `mamba`:

```
mamba install pysolar
```

It is possible to list all of the versions of `pysolar` available on your platform with `conda`:

```
conda search pysolar --channel conda-forge
```

or with `mamba`:

```
mamba search pysolar --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search pysolar --channel conda-forge

# List packages depending on `pysolar`:
mamba repoquery whoneeds pysolar --channel conda-forge

# List dependencies of `pysolar`:
mamba repoquery depends pysolar --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [Anaconda-Cloud](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating pysolar-feedstock
==========================

If you would like to improve the pysolar recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/pysolar-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@robintw](https://github.com/robintw/)

