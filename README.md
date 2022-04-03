sudo yum install git

git --version

git init 

git add singlefile.ext

git add .

git status


//////
git commit -m 'changed sample'

git push


git branch -a

to delete all files in cashed  (  git rm -r .  )

git config --global user.name 'name'
git config --global user.email 'email' 



Step 1: From your project repository, bring in the changes and test.

git fetch origin
git checkout -b foldername origin/branchname
git merge master
Step 2: Merge the changes and update on GitHub.

git checkout master
git merge --no-ff branchname
git push origin master
