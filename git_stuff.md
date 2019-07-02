#### Create a new branch off master
```
git checkout master
git pull origin master
git submodule update --init --recursive
git checkout -b <patch/feature>/CCLE-<ticket#>-<short-ticket-description>
```
#### Commit files you changed
```
git status
git add <file1> <file2> ... <filex>
git commit -m "CCLE-#### - A useful short comment summarizing what you did."
```
