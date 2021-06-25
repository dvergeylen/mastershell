---
layout: default
title: "hg remove"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-remove">
  <a href="/en/common/hg-remove.html">hg remove</a> <a href="#hg-remove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove specified files from the staging area.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#remove>.

#### Remove files or directories from the staging area:
```shell
hg remove {{path/to/file}}
```
#### Remove all staged files matching a specified pattern:
```shell
hg remove --include {{pattern}}
```
#### Remove all staged files, excluding those that match a specified pattern:
```shell
hg remove --exclude {{pattern}}
```
#### Recursively remove sub-repositories:
```shell
hg remove --subrepos
```
#### Remove files from the repository that have been physically removed:
```shell
hg remove --after
```
{% endraw %}