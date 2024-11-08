## Creating repo

* `bdsim/.github/bim/copy_reference_files.sh BDSIMBUILD TESTDATA`
* `cd testdata`
* `git lfs track "*.root"`
* `git add .gitattributes`
* `find ./ -name "*.root" -exec git add {} \;`

