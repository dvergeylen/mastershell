---
layout: default
title: "gitsome"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gitsome">
  <a href="/en/common/gitsome.html">gitsome</a> <a href="#gitsome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A terminal-based interface for GitHub, accessed via the `gh` command.
> It also provides menu-style autocomplete suggestions for `git` commands.
> More information: <https://github.com/donnemartin/gitsome>.

#### Enter the gitsome shell (optional), to enable autocompletion and interactive help for Git (and gh) commands:
```shell
gitsome
```
#### Setup GitHub integration with the current account:
```shell
gh configure
```
#### List notifications for the current account (as would be seen in https://github.com/notifications):
```shell
gh notifications
```
#### List the current account's starred repos, filtered by a given search string:
```shell
gh starred "{{python 3}}"
```
#### View the recent activity feed of a given GitHub repository:
```shell
gh feed {{tldr-pages/tldr}}
```
#### View the recent activity feed for a given GitHub user, using the default pager (e.g. `less`):
```shell
gh feed {{torvalds}} -p
```
{% endraw %}