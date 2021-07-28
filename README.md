# probable-guide
My CLI CheatSheet

## Git

### Lingo
#### Origin
Origin === probable-guide.github.com. Origin is a variable which points to the URL which stores the remote repo

#### Remote
A repo in the cloud. `origin` points to the remote repo

  &nbsp;&nbsp;

### Basic git commands
#### Download repo
`git clone https://github.com/peter-yeh/ComputerOS.git`

#### Get change from github
`git pull`

#### Check status of current branch
`git status`

#### See the commit log
`git log`

#### See the commit tree
`git log --graph`

#### Stage all changes
`git add .`

#### Commit the changes
`git commit -m 'First commit'` 

#### Push the commits to github
`git push`

&nbsp;&nbsp;

### Working in different branches

#### Create a new branch
`git checkout -b "dev-yuki`

#### Checkout from the original branch
`git checkout dev`

#### Get change from github
`git pull`

#### Back to own branch
`git checkout dev-yuki`

#### Merge all changes
`git merge dev`

<a href="https://www.atlassian.com/git/tutorials/using-branches/git-checkout">Git Checkout</a>

  &nbsp;&nbsp;

### Stash
#### Create a stash with the name
`git stash save "stash message"`

#### Stash uncommitted files
`git stash -u`

#### Check the stashes
`git stash show`

#### List the stash
`git stash list`

#### Reapply the stash
`git stash pop`

  &nbsp;&nbsp;
  
### Git merging files
#### Merge feature branch into current branch
`git merge feature` // call in master branch

##### Abort merge conflict
`git merge --abort`

  &nbsp;&nbsp;
  
### Git editing history
#### Un commit commits in git history
`git reset HEAD^`

##### Discard all non committed files
`git clean -df`

#### Remove non staged files
`git restore .`

#### Update the git repo in origin after changing the commit tree
`git push origin +HEAD`

  &nbsp;&nbsp;

## SSH
### Move **files** from local storage to remote location, e.g. sunfire
`scp lab1.tar.gz yuchun@sunfire.comp.nus.edu.sg:lab1.tar.gz`

### Move **folder** from sunfire to xcne5, -r
`scp -r lab1.tar.gz yuchun@xcne5:lab1.tar.gz`

  &nbsp;&nbsp;

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

