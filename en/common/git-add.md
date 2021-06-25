---
layout: default
title: "git add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-add">
  <a href="/en/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Adds changed files to the index.
> More information: <https://git-scm.com/docs/git-add>.

#### Add a file to the index:
```shell
git add {{path/to/file}}
```
#### Add all files (tracked and untracked):
```shell
git add -A
```
#### Only add already tracked files:
```shell
git add -u
```
#### Also add ignored files:
```shell
git add -f
```
#### Interactively stage parts of files:
```shell
git add -p
```
#### Interactively stage parts of a given file:
```shell
git add -p {{path/to/file}}
```
#### Interactively stage a file:
```shell
git add -i
```
{% endraw %}