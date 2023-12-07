# Git Branching Cheat Sheet

## Overview

Summary of commonly used git commands and practice with branching.


## Basic Commands
* `git init` - initializes local git repository
* `git add . ` - this adds everything for tracking, moves files into staging area
* `git commit -m "msg"` - this commits an entry with a message
* 

## Informational Commands
* `git log` - this shows you your prior commits on your local repository
* `git log --oneline` - this shows you your prior commits on your local repository but compact format
* `git status` - shows the state of the local working directory
* `git config -l` - this shows you the local git configuration
* `git branch -m main` - this changes the name of branch to main or to any value you want to use
* `git version` - shows the version of git you are using
* `git help` - show synopsis of git commands

## Branching Commands
* `git branch` - list local branches
* `git branch branchName` - create local branch `branchName`
* `git checkout branchName` - moves to the branch `branchName`

## Remote Commands
* `git remote add origin URL` - set `origin` as alias for remote repo `URL`
* `git push origin branchName` - push local commits to `origin` repo on branch `branchName`

