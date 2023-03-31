# Git instruction

<img src="Images/git.png" alt="git logo" width="70" height="50">

## Introduction

Git is a free and open source distributed version control system.

# Chapter I - base functionality

This section describes the basic functionality

## Starting work with Git

* To add project to source controle use command:

        git init

* To check status of repository and if any unstaged changes are in place use command:

        git status
it is a common practise to use "git status" command as soon as any changes take a place in project to check if commit is needed

## Adding files to version control

* To add file for commit use command:

        git add <filename>

* To commit changes use command:

        git commit

then enter commit message in terminal

* To add all files from the project for commit use command:

        git commit -a
then enter commit description, you should not use git add command in this case

* To commit changes jointly with commit description use command:

        git commit -m "message"

* To add all files from the project and commit them with commit description use command:

        git commit -am "message"

## Commits review

* to review commits tree with detailed information use command:

_(this command will show all commits down from the current position)_

                git log

* to review short log of commits use command:

_(this command will show all commits down from the current position)_

                git log --oneline

* to review commits tree with detailed information use command:

_(this command will show all commits up and down from the current position)_

                git log --all

* to review short log of commits use command:

_(this command will show all commits up and down from the current position)_

                git log --oneline --all


## Commits comparison

## Navigation through commits

***

<center><img src="Images/tree.jpg" alt="tree logo" width="50" height="30"></center>

<center><h1> Chapter II - Branching</h1></center>

## Introduction

## Base functionality
<p>* to create new branch use command:

                git branch <branchname>
</p>

<p>*to show all barches created use command:

                git branch
</p>

<p>*to delete branch use command:

                git branch -d <branchname>

_this command allow to delete only merged branches_
</p>

<p>
*to delete unmerged branches (over words unsaved) use command:

                git branch -D <branchname>
</p>

## Navigate through branches

<p>* to change active branch use commad:

                git checkout <branchname>
</p>

## Branches merging and conflicts

<p> *to merge working branch into the parent branch you should checkout to parent branch and use command:

                git merge <branchname>
_there branchname is a name of incoming branch_
<p>

* Merging conflicts is an event appear if both merging branches has different information in same blocks/lines of code (text) & etc.

* to solve merge conflicts during merging process choose correct information source. It could be information from incoming branch or you prefer to keep information from current branch or both.
</p>