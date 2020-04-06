---
layout: default
title: Collaboration
nav_order: 4
---

# Collaboration
{: .no_toc }

Git is a powerful tool because it allows developers to work on the same project, remotely. Multiple users can access the same Git repository through the action of cloning, or copying, a repository locally and then pushing their updates to the shared (main) repository.
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


## Cloning a Repository

To clone a repository, you must navigate in Terminal to the folder location where you want the cloned directory to appear. You will also need the URL of the repository you are going to clone:
 
```bash
git clone <repo-URL>
```

## Sharing Updates

There are two ways of downloading content from a remote repo: git fetch and git pull. git fetch will download remote content and leave the files in your local repository untouched. git pull downloads remote content and immediately merges it with your local files. 

## Pushing Updates

Push your own code to a remote repo by entering: 
```bash
git push -u <remote_name> <local_branch_name>
```

## Introduction to Branching

Git branching allows users to pull from the ‘master’ (original) branch, make changes, and only merge those changes with the ‘master’ branch when ready. It also allows users to collaborate with other users, pushing and pulling updates between users, apart from the ‘master’ branch. 

The ‘master’ branch is considered to be code that is ready for production, in contrast to development code in the ‘develop’ branch. Aside from the ‘master’ and ‘develop’ branches, there are ‘feature’, ‘release’, and ‘hotfix’ branches. Each type of branch has a specific purpose and is bound to a particular origin branch and merge target. For our purposes, we will be talking about creating a ‘feature’ branch

See what branches already exist:
```bash
git branch
```

## Create a New Local Branch

To branch off from the master, create a new branch: 

1.  Create and name your new branch: 
```bash
git branch <new-branch-name>
```
2.  Rename branch: 
```bash
git previous-branch-name -m <new-branch-name>
```

## Merge Branch to a Remote Repository

To add a branch to a remote repository:

1.  Add a remote repo to local repo configuration: 
```bash
git remote add <new-remote-repo-name> <repo-URL>
```
2.  Push new branch to remote repo: 
```bash
git push <new-remote-repo-name> <new-branch-name>~
```

## Delete a Branch

A branch is no longer needed once it and its history has been merged with the master. To delete a branch locally:

1.  Ensure branch has been merged, otherwise an error message will appear when attempting to delete.
2.  Delete after merging: 
```bash
git branch -d <new-branch-name>
```
3.  Delete without merging (in the event that you are discarding the development): 
```bash
git branch -D <new-branch-name>
```

To delete a remote branch, execute: 
```bash
git push origin --delete <new-branch-name>
```

## Completed all the steps?
{: .no_toc }

You will know if you have entered an incorrect command or not achieved the goals of this instruction set if you see any Terminal error messages. If so, please try the steps again or visit our ‘Troubleshooting’ page.
