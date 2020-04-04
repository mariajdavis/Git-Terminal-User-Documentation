---
layout: default
title: Create a Repository
nav_order: 2
---

# Configuration
{: .no_toc }


To get started using Git on Terminal, you will want to familiarize yourself with basic Terminal commands, install Git, set up a Git account and a default text editor.
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Basic Terminal Commands

The following basic Terminal commands will allow you to navigate your computer’s working directory. Some of them will be used in this user documentation:

Note: Whenever the <> symbols appear in a command, it is meant to be replaced with your own input.

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


Note: You will know when Git has been successfully installed when the ```bashgit --version```	command the following result appears in Terminal: ```bashgit version <latest-version-number> (Apple Git-<version-number>)```

## Initialize Account

```yaml
# Aux links for the upper right navigation
aux_links:
  "Just the Docs on GitHub":
    - "//github.com/pmarsceill/just-the-docs"
```

## Text Editor

```yaml
# Heading anchor links appear on hover over h1-h6 tags in page content
# allowing users to deep link to a particular heading on a page.
#
# Supports true (default) or false/nil
heading_anchors: true
```



