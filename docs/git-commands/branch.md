---
sidebar_position: 3
---

# Branch

The branch git command allows for you to manipulate and view information about existing git branches in the local repository

## Get names of branches and see which is active

To get the names of all branches in the local repository simply use the `git branch` command as seen below:

```
$ git branch
  01-github-guidelines
* 02-git-commands
  main
```

As can be seen it names the three branches of the local repository and also places an asterisk next to the branch that is currently active.

## Rename a local branch

There may be a situation where the name of a branch needs to be changed; in this situation you can include the `-m` flag in order to change the name of the current branch:

`git branch -m <new-branch-name>`

An example is shown below where the branch previously named `rename-me` is changed to `new-name`

```
$ git branch
  01-github-guidelines
  02-git-commands
  main
* rename-me

$ git branch -m new-name

$ git branch
  01-github-guidelines
  02-git-commands
  main
* new-name
```

## Delete a local branch

To delete a no longer needed local branch from your local repository use the `-d` flag followed by the name of the branch to delete:

```
$ git branch
  01-github-guidelines
* 02-git-commands
  main
  new-name

$ git branch -d new-name
Deleted branch new-name (was 68561b7).

$ git branch
  01-github-guidelines
* 02-git-commands
  main
```

NOTE: You may want to retain old branches for some time after they seem to no longer be needed to make sure that deleting them is ok to do.