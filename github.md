# Version Control

Version control is a system that allows you to go back to various versions of a file or set of files by recording your changes. You can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes. 

**Local version control** entails one database on your hard disk that stores changes to files.

**Centralized version control system** (CVCS) is a system that entails a single server storing all changes and file versions, that can be accessed by various clients.

**Distributed version control system** (DVCS) is a system that allows clients to create mirrored repositories. This is in place so if a CVS goes down or a central database's hard disk gets corrupted, all work will not be lost and you can still collaborate if working in a team. Allows you to create data backups.

# What is Git?

Git is a DVCS that stores data in a file system made up of snapshots. Any time you save a changed version of the project (AKA commit) Git creates a snapshot of the file and stores a reference to it. Git mostly relies on local operations since most necessary information can be found locally. This allows for expediency because a project's history resides on the local disk, elimating need to fetch history information from the server. Also allowing one to continue work on a project even when offline or on a VPN. Git will always detect file corruption or loss of information in transit.

## Setting up a Git Repository

To import an existing project or directory into Git:
1. Switch to the target project's directory
**Ex:** $ cd test
2. Use the git init command
**Ex:** $ git init
_You have created a new subdirectory named .git that has the repository files._
3. To start tracking these files, perform a commit by typing:
$ git add *.c
$ git add LICENSE
$ git commit -m "your message"

You can also create copies of existing Git repositories.
**Ex:** $ git clone https://github.com/test

By cloning, you have copied all versions of all files for the project.

The local Git repository has three componets:
1. working directory (actual files reside here)
2. index (area used for staging)
3. head (points to the most recent commit)

**Tracked** files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
**Untracked** files were not in the last snapshot and do not currently reside in the staging area. After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.
## File Status

![](https://github.com/connorrrrrrr/reading-notes/blob/main/lifecycleoffilestatus.png)
To determine the state of files, use **git status**. To track 1 file, use **git add filename**. To track all files in a repository use, **git add asterik**.

**git commit -a** commits a snapshot of all modifications to tracked files in the working directory.

**git push origin main** pushes changes from the local "main" branch to the remote repository named "origin". For cloned repositories, Git will automatically give the name "origin" to the server from which you cloned and the name "main" to your local repository. These names can be changed by the user.

## Stashing Changes

When you are not ready to commit changes but do not want to lose them either, **git stash** is a great option. This temporarily removes changes and hides them, giving you a clean working directory. When you're ready to continue working on changes, simply use **git stash apply** to retrieve the hidden changes.
### Remote Repositories

To collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges.

[<===Home](README.md)