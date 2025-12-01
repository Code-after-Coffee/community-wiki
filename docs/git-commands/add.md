---
sidebar_position: 7
---

# Add

The git add command is used to stage changes in a local repository that will be saved into the next commit made.

Staging is a process of selecting which files/changes to files will be included in the next commit message made.

## Adding a single file

To add only a single file in the local repository use `git add <file-name>` where `file-name` is the name of the file including any directories that are needed to reach the file from the current location that the terminal is running the command from.

## Adding all files in a directory

To add all files in the current directory of the local repository use `git add .`

## Adding all modified files in the respository

To add all modified files in the entire local repository use the `-u` flag:

`git add -u`

## Adding all changes in the entire repository

To add all changes in the entire local repository including new/renamed/deleted files use the `-A` flag

`git add -A`

<!-- TODO: enchance add with interactive mode commands for block staging -->