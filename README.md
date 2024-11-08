## Creating repo

* `bdsim/.github/bim/copy_reference_files.sh BDSIMBUILD TESTDATA`
* `cd testdata`
* `git lfs track "*.root"`
* `git add .gitattributes`
* `find ./ -name "*.root" -exec git add {} \;`

## Other than root files

* `git lfs track "*.FILEXTENSION"`

## Adding files

Just add, commit, push large files as normal

* `git add LARGEFILE`
* `git commit LARGEFILE -m "message"`

