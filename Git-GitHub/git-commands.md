# Git Guide

Check out: https://docs.github.com/en/get-started/using-git/about-git

## What is Git?

Git is a distributed version control system that tracks all the changes that are made to a project and that lets you view the hístory of changes and recover earlier versions of the project.

Git makes use of repositories. A repository is a collection of all files and folders that are associated with a project.  
Everytime you make changes in the repo and commit those changes, git will take a snapshot of the repo.  
A git repo will track all the commits that are made.

## Git commands

"git init"  
initalizes a new git repo. A hidden subfolder called git will be added, to keek track of all the changes.

"git clone"
creates a local copy of a project that already exists remotely.

"git add"  
stages a change (Unclear what is staging?)

"git commit"
saves a snapshot of the repo and adds it to the tracked changes.

"git branch"  
shows all local branches (git branch -a also shows remote branches).

"git merge"  
combines changes in different branches

"git pull"  
uodates the local repo with changes from the remote repo.

"git push"  
updates the remote repo with changes from the local repo.
