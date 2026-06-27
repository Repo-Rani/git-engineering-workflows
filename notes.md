Class-1

Install git and github
we have a tow types of repo in this 
1) git local repo
2) github remote repo

1) configuration for connect git with your github account:
git config --global user.name "Write Here UserName From Github Account"

2) configure you git email with the same github account email:
git config --global user.email "Write Here same Email From Github Account"

3) Git Configuration List Command is
git config --list

class-2

1) To push your working directory do these steps one by one:
step-1: create repositry in a github Web Host
step-2: git init (For git initialization in a working dircetory ) 
step-3: git add file name or . (For tracking changes of files / or Maintain History Of These Files)
step-4: git commit -m "Write Here Message for Commit" (To store code in a local git repositry)
step-5: git branch -M main (For main Branch / By default Github branch name is main/ for Branch name Rename)
step-6: git remote add origin "Url for Github repo" (To push working dir in a remote repositry)
step-7: git push origin -u main (To push code in a remote repo/ -u To async local branch from remote branch)

