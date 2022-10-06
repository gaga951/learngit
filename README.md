$ sudo yum install git

$ git --version

$ git init 

$ git add singlefile.ext

-----

### to set username and email global parameters for our system

$ git config --global user.name 'name'

$ git config --global user.email 'email' 

### to clone remote repository in your local folder

$ git clone https://repourl

### To initialize as remote repo in our current folder 

$ git remote add origin https://repourl

### we can check curent config file

vi .git/config

### To chek perrmisions we have in remote repo

git remote -v


### add multiple file wich starts with same specific name

$ git add specificname*

-----

$ git add .

$ git status


//////
$ git commit -m 'changed sample'

git log

git log -p

git show <commit hash code>

### Single line format:

git log --pretty=oneline

### other display of entries

git log --pretty=oneline --max-count=2
  
git log --pretty=oneline --since='5 minutes ago'
  
git log --pretty=oneline --until='5 minutes ago'
  
git log --pretty=oneline --author=<your name>
  
git log --pretty=oneline --all


$ git push
  
  
  
### To create new branch 
  
$ git branch newbranchname
  
### If i am in master branch I can merge newbranch to master branch using command
  
$ git merge newbranchname
  
### To delete branch 
  
$ git branch -d newbranchname  

### To see list of braches
  
$ git branch -a

### to delete all files in cashed

$ git rm -r .

### to unstage specific file

$ git rm --cached filename
  
### After editing changes to already commited file, we can undo file changes
  
$ git restore filename
  
  or
  
$ git checkout filename
 
-------
  
### If accedentally deleted file via 
  
$ git rm filename 
  
### we can revert it by
  
$ git restore --stage filename
  
$ git restore filename  
  
-------




### Step 1: From your project repository, bring in the changes and test.

$ git fetch origin

$ git checkout -b foldername origin/branchname

$ git merge master

### Step 2: Merge the changes and update on GitHub.

$ git checkout master

$ git merge --no-ff branchname

$ git push origin master



### ---------------------------------------------
### Aliases for Windows:

RUN:
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.st status
git config --global alias.br branch
git config --global alias.hist "log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short"
git config --global alias.type 'cat-file -t'
git config --global alias.dump 'cat-file -p'

---------------------------------------------

### Aliases for Unix/Mac:

git status, git add, git commit, and git checkout are common commands so it is a good idea to have abbreviations for them.

Add the following to the .gitconfig file in your $HOME directory.
  
### 
 /*
FILE: .GITCONFIG
[alias]
  co = checkout
  ci = commit
  st = status
  br = branch
  hist = log --pretty=format:\"%h %ad | %s%d [%an]\" --graph --date=short
  type = cat-file -t
  dump = cat-file -p
*/
---------------------------------------------

