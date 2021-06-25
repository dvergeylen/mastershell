---
layout: default
title: "hg clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-clone">
  <a href="/en/common/hg-clone.html">hg clone</a> <a href="#hg-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a copy of an existing repository in a new directory.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#clone>.

#### Clone a repository to a specified directory:
```shell
hg clone {{remote_repository_source}} {{destination_path}}
```
#### Clone a repository to the head of a specific branch, ignoring later commits:
```shell
hg clone --branch {{branch}} {{remote_repository_source}}
```
#### Clone a repository with only the `.hg` directory, without checking out files:
```shell
hg clone --noupdate {{remote_repository_source}}
```
#### Clone a repository to a specific revision, tag or branch, keeping the entire history:
```shell
hg clone --updaterev {{revision}} {{remote_repository_source}}
```
#### Clone a repository up to a specific revision without any newer history:
```shell
hg clone --rev {{revision}} {{remote_repository_source}}
```
{% endraw %}