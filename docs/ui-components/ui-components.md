---
layout: default
title: Repositories
nav_order: 3
---

# Repositories
{: .no_toc }


A Git repository is a folder that virtually stores a project. It is the . git/ folder inside a project folder on your computer. This repository tracks all changes made to files in the project, allowing developers to view project history. 
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Create a Repository for an Existing Project

To create a repository, you will first need to navigate to the correct location in your working directory via Terminal. 

To create a repository for an existing project:

1. View contents of your computer’s root directory in Terminal: 
```bash
ls
```
2.  Enter the directory containing the project:
```bash
cd <folderName>
```
3.  Initialize the new repository: 
```bash
git init
 ```
4.  Add any new files in the directory: 
```bash
git add
```

|   ![Icon](https://imgur.com/8hOhnYk.png) | It is highly recommended to leave clear and concise commit messages. It will be much more helpful when you need to go back and find a previous version if you have clear indications of what you changed in each commit |

5.  Commit new files: 
```bash
git commit -m “commit message goes here”
```

## Create a Repository for a New Project

To create a repository for a new project that has not yet been started:

1.  In the directory location of your choice, enter: 
```bash
mkdir <new-directory-name>
```
2.  Go into the new directory: 
```bash
  cd <new-directory-name>
```
3.  Execute: 
```bash
  git init
```

## Update a Repository

To update a local repository, users are required to add and commit files:

1.  Make sure you are in the correct directory: 
```bash
cd <path/to/project>
```
2.  Create a new file with some contents (“testing commit function”) and label it testCommit.txt : 
```bash
echo “testing commit function” >> testCommit.txt
```
3.  Add new file to the repository staging area:
```bash
git add testCommit.txt
```
4. Commit new files: 
```bash
git commit -m “write a professional commit message”
```

|   ![Icon](https://imgur.com/8hOhnYk.png) | To push your work to (share it with) a remote repository, you will need to use a Git host service to store your repository. The service will provide you with a URL that you can use to push your code. GitHub is our preferred Git host service: https://github.com/ |

5.  Add a remote repository to your local git configuration using: 
```bash
git remote add <remote_name> <remote_repo_url>
```

## Conclusion

You will know if you have entered an incorrect command or not achieved the goals of this instruction set if you see any Terminal error messages. If so, please try the steps again or visit our ‘Troubleshooting’ page.
