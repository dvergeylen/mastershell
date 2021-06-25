---
layout: default
title: "hg add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-add">
  <a href="/en/common/hg-add.html">hg add</a> <a href="#hg-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Adds specified files to the staging area for the next commit in Mercurial.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#add>.

#### Add files or directories to the staging area:
```shell
hg add {{path/to/file}}
```
#### Add all unstaged files matching a specified pattern:
```shell
hg add --include {{pattern}}
```
#### Add all unstaged files, excluding those that match a specified pattern:
```shell
hg add --exclude {{pattern}}
```
#### Recursively add sub-repositories:
```shell
hg add --subrepos
```
#### Perform a test-run without performing any actions:
```shell
hg add --dry-run
```
{% endraw %}