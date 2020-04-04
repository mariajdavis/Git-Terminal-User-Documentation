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


View this site's [_config.yml](https://github.com/pmarsceill/just-the-docs/tree/master/_config.yml) file as an example.

## Basic Terminal Commands

The following basic Terminal commands will allow you to navigate your computer’s working directory. Some of them will be used in this user documentation:

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

```yaml
# Enable or disable the site search
# Supports true (default) or false
search_enabled: true

# Enable support for hyphenated search words:
search_tokenizer_separator: /[\s/]+/

```

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



