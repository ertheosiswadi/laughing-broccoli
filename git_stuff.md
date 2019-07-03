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
### Squashing commits
[Reference](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html)
```
git rebase -i HEAD~<# of commits you want to squash>
```
#### Example: 4 commits
```
pick 01d1124 Adding license (oldest)
pick 6340aaa Moving license into its own file
pick ebfd367 Jekyll has become self-aware.
pick 30e0ccb Changed the tagline in the binary, too. (newest)
```
Use the editor to change from pick → squash except the oldest commit
```
pick 01d1124 Adding license
squash 6340aaa Moving license into its own file
squash ebfd367 Jekyll has become self-aware.
squash 30e0ccb Changed the tagline in the binary, too.
```
Another editor will pop out for the commit message, just choose one or make one that follows this format:
>"CCLE-#### - A useful short comment summarizing what you did."

