---
sidebar_position: 4
---

# Checkout

The git checkout command allows for switching or creating branches in the local repository on your machine

## Switch to an exisiting branch

To switch to an already existing branch in the local repository use `git checkout <branch-name>`

```
$ git branch
  01-github-guidelines
* 02-git-commands
  main

$ git checkout 01-github-guidelines
Switched to branch '01-github-guidelines'
Your branch is up to date with 'origin/01-github-guidelines'.

$ git branch
* 01-github-guidelines
  02-git-commands
  main
```

## Create a new branch

To create a new branch in the local repository and switch to it use the `-b` flag: 

```
$ git branch
* 01-github-guidelines
  02-git-commands
  main

$ git checkout -b new-branch
Switched to a new branch 'new-branch'

$ git branch
  01-github-guidelines
  02-git-commands
  main
* new-branch
```