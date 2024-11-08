## Introduction

LFS file repo for storing bdsim reference output files. Should be tagged with new bdsim versions. Directory structure
is exactly the same as a examples/test directories in bdsim


## Creating BDSIM reference files

* `cd BDSIM_BUILD`
* `cmake ../BDSIM_SRC -DBDSIM_GENERATE_REGRESSION_DATA=ON`
* `BDSIM_SRC/.github/bin/copy_reference_files.sh BDSIM_BUILD BDSIM_TESTDATA`
* `cd BDSIM_TESTDATA`
* `git add -A`
* 'git commit -a -m "Update reference test data"

## Other than root files

* `git lfs track "*.FILEXTENSION"`

## Adding files

Just add, commit, push large files as normal

* `git add LARGEFILE`
* `git commit LARGEFILE -m "message"`

## Creating repo

* `bdsim/.github/bim/copy_reference_files.sh BDSIMBUILD TESTDATA`
* `cd testdata`
* `git lfs track "*.root"`
* `git add .gitattributes`
* `find ./ -name "*.root" -exec git add {} \;`

