# TRISTAN/rb_cva6_cropro_crc
This repository is holding the source RTL for the copro CRC designed by Bosch, in the contest of the TRISTAN project.
Additionnaly, some testbenches are available.
The design flow is also run on the copro from this repository, if needed.

## Table of Contents <!-- omit in toc -->
- [How to use this repo](#howto)
- [Directory Structure](#directory-structure)
- [Links and resources](#links-resources)
- [About](#about)
  - [Maintainers](#maintainers)

## How to use this repo <a name="howto"></a>

This repository cannot be used standalone and require a tada environment and other associated repos.
To setup a working environment do the following
```
tada -new my/tristan_fe/my_workspace
repoinit
repo sync
## This is needed to load the module tools as it is not done automatically during the tada creation
tada -exit
tada my/tristan_fe/my_workspace
libgen.sh
```
By default, it is the master branch that is available. All changes should be done
on a branch, derived from the develop branch. A branch should be limited to one bugfix or improvement/modification.
Develop and master branches can only be modified through pull request with a review process.
A more detailed explanation of the branching model is available on [Docupedia](https://inside-docupedia.bosch.com/confluence/display/TRISTAN/TRISTAN+Home)

To work on a feature on this repository :
```
git fetch
git checkout -b my_feature bitbucket/my_feature
```

## Directory Structure <a name="directory-structure"></a>

This repository is structured according to the standard EIY folder structure :
* rtl_v : contains RTL files
* test_c : contains C files used for tests **(To be filled)**
* tb_v : contains testbench files **(To be filled)**
* scripts : Makefiles to run the testbenches **(To be filled)**
* saxo : Makefile and setup scripts for packaging with the SAXO tool, in particular for xcelium_check **(To be filled)**

## Links and resources <a name="links-resources"></a>
* [EU TRISTAN project description](https://cordis.europa.eu/project/id/101095947)
* [Getting started with git and bitbucket](https://inside-docupedia.bosch.com/confluence/x/CArpCw)
* [TRISTAN docupedia](https://inside-docupedia.bosch.com/confluence/display/TRISTAN/TRISTAN+Home)
* [TRISTAN bitbucket](https://sourcecode.socialcoding.bosch.com/projects/TRISTAN)
* [CRC Copro specification](https://sourcecode.socialcoding.bosch.com/projects/TRISTAN/repos/repo_tristan/browse/Specs/CV32a6_embedded_WI2.4.5/documents/design_specification)

## About <a name="about"></a>
Together for RISc-V Technology and ApplicatioNs (TRISTAN) is a project financed partly by the Europan Union and involving multiple companies.
Some of the activities done by BOSCH will by open-sourced while other aspects will stay closed source.

### Maintainers <a name="maintainers"></a>

* [ALLIOUX Coralie](coralie.allioux@fr.bosch.com)
* [BETSCHI Olivier](olivier.betschi@fr.bosch.com)
* [BLANCHARD Ludovic](ludovic.blanchard@fr.bosch.com)
