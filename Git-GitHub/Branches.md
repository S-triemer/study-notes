# Branches

## What are Branches

A branch helps to isolate your code without affecting other branches in the repo

## Workflow

### Create a new local branch from the command line

Inside the local repo use:
"git branch branchname"  
to create a branch with the name "branchname".

### Start working on the new branch

Inside the local repo use:
"git checkout branchname"  
this will change your working branch to the branch with the name "branchname". All changes in the code are now done on this branch.

### Add the branch to the remote repository

To make the branch available in the remote repo use:
"git push origin branchname"  
This will add the branch with the name of branchname to the remote repo

### Merge the changes

When you're satisified with your work, you can merge the changes from the current branch to another branch.

#### Merging locally

To merge changes locally, you can navigate to the branch that you would like your changes to be merged to eg. main and than use:  
"git merge branchname"  
This will merge all the changes from "branchname" to main.
After the branch is merged, you can use:  
"git branch -d branchname"  
to delete the branch with the name of branchname.

#### Merging with someone elses codebase

Push your changes to your cloned repo on github by using:  
"git push origin branchname"  
This will push the branch with the name of branchname to the github repo.

Afterwards create a pull request to get your changes merged:  
How to create pull requests: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
