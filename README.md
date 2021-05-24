# probable-guide
My CLI CheatSheet

## Git
#### Download repo
`git clone https://github.com/peter-yeh/ComputerOS.git`

#### Get change from github, do it before making changes to get the latest update
`git pull`

#### Check status of current branch
`git status`

#### Stage all changes
`git add .`

#### Add All changes
`git commit -m 'First commit'` 

#### Push all changes to github
`git push`

#### Merge
`git merge feature` // call in master branch

#### Stash
`git stash save "stash message"`

`git stash show`

`git stash -u` // stash untracked(uncommitted) files too

`git stash list`

`git stash pop` // reapply the stash

## SSH
### Move **files** from local storage to remote location, e.g. sunfire
`scp lab1.tar.gz yuchun@sunfire.comp.nus.edu.sg:lab1.tar.gz`

### Move **folder** from sunfire to xcne5, -r
`scp -r lab1.tar.gz yuchun@xcne5:lab1.tar.gz`


## Useful Unix commands
### Compile c code into exe format
`gcc ex1.c -o ex1.exe`

### Pass text in test1.in into ex1.exe
`./ex1.exe < test1.in`

`./ex1.exe < test1.in > myOut1.txt`

### Comparing files
`diff test1.out myOut1.txt`

### Unzip the zip files
`gunzip -c lab1.tar.gz | tar xvf -`

### Remove whole folder (-r recusrive)
`yes | rm -r folder` // for sunfire since it keeps asking confirmation

`rm -r folder` // for xcne

