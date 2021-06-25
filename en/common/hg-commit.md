---
layout: default
title: "hg commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-commit">
  <a href="/en/common/hg-commit.html">hg commit</a> <a href="#hg-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commit all staged or specified files to the repository.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#commit>.

#### Commit staged files to the repository:
```shell
hg commit
```
#### Commit a specific file or directory:
```shell
hg commit {{path/to/file_or_directory}}
```
#### Commit with a specific message:
```shell
hg commit --message {{message}}
```
#### Commit all files matching a specified pattern:
```shell
hg commit --include {{pattern}}
```
#### Commit all files, excluding those that match a specified pattern:
```shell
hg commit --exclude {{pattern}}
```
#### Commit using the interactive mode:
```shell
hg commit --interactive
```
{% endraw %}