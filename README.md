$ sudo yum install git

$ git --version

$ git init 

$ git add singlefile.ext

-----

### add multiple file wich starts with same specific name

$ git add specificname*

-----

$ git add .

$ git status


//////
$ git commit -m 'changed sample'

git log

### Single line format:

git log --pretty=oneline

### other display of entries

git log --pretty=oneline --max-count=2
git log --pretty=oneline --since='5 minutes ago'
git log --pretty=oneline --until='5 minutes ago'
git log --pretty=oneline --author=<your name>
git log --pretty=oneline --all


$ git push

$ git branch -a

### to delete all files in cashed

$ git rm -r .

### to unstage specific file

$ git rm --cached filename

### to set username and email global parameters for our system

$ git config --global user.name 'name'

$ git config --global user.email 'email' 


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

