---
layout: default
title: Getting Started
nav_order: 2
---

# Getting Started
{: .no_toc }


To get started using Git on Terminal, you will want to familiarize yourself with basic Terminal commands, install Git, set up a Git account and a default text editor.
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Basic Terminal Commands

The following basic Terminal commands will allow you to navigate your computer’s working directory. Some of them will be used in this user documentation:

**Note: Whenever the <> symbols appear in a command, it is meant to be replaced with your own input.**

Change directory:
```bash
cd <path/to/directory/>
```

Move backwards a directory:
```bash
cd ..
```

List contents of directory:
```bash
ls "path/to/directory/" 
```

Open a file:
```bash
open <filename> 
```

Create a directory:
```bash
mkdir <new-directory-name> 
```

## Git Installation

To install Git:

1.  Open the Terminal application
2.  Check to see if git is already installed: 
```bash
git --version
```
3.  If it is not yet installed, you will be prompted to go ahead and install it


**Note: You will know when Git has been successfully installed when the ```bashgit --version```	command the following result appears in Terminal: ```bashgit version <latest-version-number> (Apple Git-<version-number>)```**

## Initialize Account

Configure your account by entering a username and email that you want to be associated with all activity through your account: 

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

**Note: The ‘--global’ portion of the above two commands means you only have to enter this information once. After that, the system will associate your account with all Git activity. To override this with a different name and email address, re-enter the above two commands without ‘--global’ while working on a project.**

## Text Editor

It can be quite helpful to have access to a text editor graphical user interface through Git on Terminal. We recommend setting up Visual Studio Code (VS Code) as the default. 

**Note: Install VS Code for Mac here: https://code.visualstudio.com/docs?dv=osx**

To set up VS Code as a default text editor:

1.  Enter: 
```bash
git config --global core.editor "code --wait"
```
2.  Edit the global configuration settings in VS Code: 
```bash
git config --global -e
```

## Conclusion

You will know if you have entered an incorrect command or not achieved the goals of this instruction set if you see any Terminal error messages. If so, please try the steps again or visit our ‘Troubleshooting’ page.
