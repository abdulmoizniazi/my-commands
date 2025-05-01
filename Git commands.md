git config --global user.name "Moiz Khan"
git config --global user.email "abdulmoizniazi@gmail.com"
git config --global push.default matching
git config --global alias.co checkout
git init
git add .
git commit -am "initial commit"

git remote add origin https://github.com/abdulmoizniazi/XXXXXXX.git
git branch -M main
git push -u origin main
^
git add . 
git commit -am "remarks for every commit"
git push

git pull --rebase origin main
git push --force

git rm -r --cached node_modules
.........................................................
git status
git remote -v
git add .
git commit -m "Your updated message"
git pull origin master
(manage changes)
git commit -m "Resolved merge conflicts"
git push origin master

git checkout branch-name   git checkout -b new-branch-name
git switch branch-name     git switch -c new-branch-name
git branch        # local branches
git branch -r     # remote branches
git branch -a     # all branches
git push -u origin new-branch-name
.........................................................
.........................................................

echo "# CRM-Django" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/abdulmoizniazi/xxxxxxxx.git
git push -u origin main