#### Create a new branch off master
```
git checkout master
git pull origin master
git submodule update --init --recursive
git checkout -b <patch/feature>/CCLE-<ticket#>-<short-ticket-description>
```
