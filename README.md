
ssh <kanciab>@<host> cd path/above/repo git init --bare kanciab.git

git clone <nardzedziaprogr> <kanciab>


git config user.name <kanciab>
git config --global user.name <kanciab>


 
# Edit hello.py git status # hello.py is listed under "Changes not staged for commit" git add hello.py git status # hello.py is listed under "Changes to be committed" git commit git status # nothing to commit (working directory clean)
git log --oneline

commit 3157ee3718e180a9476bf2e5cab8e3f1e78a73b7 Author: kanciab

git log --author="kanciab" -p hello.py

 
b7119f2 Continue doing crazy things 872fa7e Try something crazy a1e8fb5 Make some important changes to hello.py 435b61d Create hello.py 9773e52 Initial import
 
 
 git checkout a1e8fb5 hello.py
 
git commit --amend

 Edit hello.py and main.py git add hello.py git commit # Realize you forgot to add the changes from main.py git add main.py git commit --amend --no-edit
 
  
# Create a hotfix branch based off of master git checkout -b hotfix master # Edit files git commit -a -m "Fix security hole" # Merge back into master git checkout master git merge hotfix git branch -d hotfix
git rebase -i


 
0a2e358 HEAD@{0}: reset: moving to HEAD~2 0254ea7 HEAD@{1}: checkout: moving from 2.2 to master c10f740 HEAD@{2}: checkout: moving from master to 2.2
 
 
 
 
