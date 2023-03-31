# Git instruction

## Introduction

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

* to comapre existing changes with last commit use command:
        
        git diff

* to compare existing last changes with exact commit use command:

        git diff <hash>

* to compare to commits use command:

        git diff <hash1> <hash2>

## Navigation through commits

* to swich commit for work use command:

        git checkout <hash>

* to return to the master commit instead of hash use command:

        git checkout master