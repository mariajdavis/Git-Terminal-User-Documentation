---
layout: default
title: Troubleshooting
nav_order: 6
---

# Troubleshooting
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Committed to Wrong Branch

If you commit an update to the wrong branch:

```bash
git reset HEAD~ --soft
git stash
git checkout correctBranchName
git stash pop
git add . # or add individual files
git commit -m "message here"
```

## Wrong Commit Message

If you need to change the message on your last commit:

```bash
git commit --amend -m "new commit message"
```


## Wrong File Added

If you need to remove a file from Git without removing it from your file system:

```bash
git reset fileName
echo file >> .gitignore
```


## Mistake Realized After Committing

If you need to make a change right after you make a commit:

1.  Make that change. 
2.  Enter: 
```bash
git add <file-name>
git commit --amend --no-edit
```

## Merge Conflict

Merge conflicts occur when Git is unable to resolve differences in code between two commits from two different users. 

If a merge conflict occurs:

1.  Find the local repository that has the conflict:
```bash
cd repo-name
```
2.  Determine what files have a merge conflict:
```bash
git status 
```
3.  Open a text editor, and go to the file with the conflict.
4.  Search for the conflict marker:
```bash
<<<<<<< HEAD
```
5.  Then you’ll see ```bash=====``` which divides the two conflicting changes.
6.  This is all followed by:
```bash
>>>>>>>BRANCH-NAME
```
7.  Decide if you want to keep your changes or delete them. 
8.  Delete the following markers: 
```bash
<<<< ==== >>>>>
```
9.  Add and commit your changes:
```bash
git add <file-name>
git commit -m “commit message”
```

