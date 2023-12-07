# Git Branching Cheat Sheet

## Overview

Summary of commonly used git commands and practice with branching.

## Summary of Branch Workflow
1. Checkout and pull main
	```bash
	git checkout main
	git pull origin main
	```
1. Checkout new branch from up-to-date main
	``` bash
	git checkout -b someFeature
	```

1. Work, committing each completed task, until feature is complete
1. Pull remote main into local branch
	```bash
	git add .
	git commit -m "complete feature"
	git pull origin main
	```

	* If auto merge succeeds, save and quit from `vi` editor:
	```
	:wq
	```

	* If `CONFLICT`, fix conflicts in all files and removing merge markers and commit
	``` bash
	git add .
	git commit -m "fix merge conflicts"
	```
1. Push to remote branch
	```
	git push origin someFeature
	 bash 
	```
1. On Github, create pull request and merge with main
1. Checkout and pull merge main
	```
	bash
	git checkout main
	git pull origin main
	```

>>>>>>> 2e19ac87428961b22fa59fdac1801725af6dae67

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
* `git checkout -b branchName` - create and move to `branchName`

## Remote Commands
* `git remote add origin URL` - set `origin` as alias for remote repo `URL`
* `git push origin branchName` - push local commits to `origin` repo on branch `branchName`
* `git pull origin main` - pull remote branch `branchName` into current local branch
