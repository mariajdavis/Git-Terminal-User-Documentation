---
layout: default
title: Introduction
nav_order: 1
description: "Introduction to Git on Terminal"
permalink: /
---

# Git on Terminal
{: .fs-9 }

User documentation for Git on Mac's Terminal
{: .fs-6 .fw-300 }

[Introduction to Git](#introduction-to-git){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Introduction to Terminal](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

---

## Purpose

This user documentation series is meant for first time users of Git on the built-in Terminal interface of Mac operating systems. This documentation will introduce users to the basic commands they will need to know to set up Git on their computer, create and manage their own Git repository, and use Git to collaborate with others.

## Introduction to Git

Git is a popular version-control system used in software development. Version-control allows  developers to track changes in source code throughout development. It also enables collaboration between developers working remotely. 

## Introduction to Terminal

Terminal is the built-in command-line interface on Mac operating systems. A command-line interface processes text commands to the computer. One way to use Git is through the command line. While there are now different graphical user interfaces that allow you to utilize Git without using Terminal, like GitHub Desktop, there are certain Git commands that can only be executed on the command line. Many employers expect developers to be comfortable working on the command line.

## Assumptions

These instructions assume that users are already familiar with their Mac operating systems and can access the Terminal interface. It will also assume that a user can prepare their own project files to store on Git.


### Quick start: Use as a GitHub Pages remote theme

1. Add Just the Docs to your Jekyll site's `_config.yml` as a [remote theme](https://blog.github.com/2017-11-29-use-any-theme-with-github-pages/)
```yaml
remote_theme: pmarsceill/just-the-docs
```
<small>You must have GitHub Pages enabled on your repo, one or more Markdown files, and a `_config.yml` file. [See an example repository](https://github.com/pmarsceill/jtd-remote)</small>

### Local installation: Use the gem-based theme

1. Install the Ruby Gem
```bash
$ gem install just-the-docs
```
```yaml
# .. or add it to your your Jekyll site’s Gemfile
gem "just-the-docs"
```
2. Add Just the Docs to your Jekyll site’s `_config.yml`
```yaml
theme: "just-the-docs"
```
3. _Optional:_ Initialize search data (creates `search-data.json`)
```bash
$ bundle exec just-the-docs rake search:init
```
3. Run you local Jekyll server
```bash
$ jekyll serve
```
```bash
# .. or if you're using a Gemfile (bundler)
$ bundle exec jekyll serve
```
4. Point your web browser to [http://localhost:4000](http://localhost:4000)

If you're hosting your site on GitHub Pages, [set up GitHub Pages and Jekyll locally](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll) so that you can more easily work in your development environment.

### Configure Just the Docs

- [See configuration options]({{ site.baseurl }}{% link docs/configuration.md %})

---

## About the project

Just the Docs is &copy; 2017-2019 by [Patrick Marsceill](http://patrickmarsceill.com).

### License

Just the Docs is distributed by an [MIT license](https://github.com/pmarsceill/just-the-docs/tree/master/LICENSE.txt).

### Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. Read more about becoming a contributor in [our GitHub repo](https://github.com/pmarsceill/just-the-docs#contributing).

#### Thank you to the contributors of Just the Docs!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul>

### Code of Conduct

Just the Docs is committed to fostering a welcoming community.

[View our Code of Conduct](https://github.com/pmarsceill/just-the-docs/tree/master/CODE_OF_CONDUCT.md) on our GitHub repository.
