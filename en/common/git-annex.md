---
layout: default
title: "git annex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-annex">
  <a href="/en/common/git-annex.html">git annex</a> <a href="#git-annex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage files with Git, without checking their contents in.
> When a file is annexed, its content is moved into a key-value store, and a symlink is made that points to the content.
> More information: <https://git-annex.branchable.com>.

#### Help:
```shell
git annex help
```
#### Initialize a repo with Git annex:
```shell
git annex init
```
#### Add a file:
```shell
git annex add {{path/to/file_or_directory}}
```
#### Show the current status of a file or directory:
```shell
git annex status {{path/to/file_or_directory}}
```
#### Synchronize a local repository with a remote:
```shell
git annex {{remote}}
```
#### Get a file or directory:
```shell
git annex get {{path/to/file_or_directory}}
```
{% endraw %}