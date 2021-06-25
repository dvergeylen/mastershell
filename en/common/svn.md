---
layout: default
title: "svn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="svn">
  <a href="/en/common/svn.html">svn</a> <a href="#svn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Subversion command-line client tool.
> More information: <https://subversion.apache.org>.

#### Check out a working copy from a repository:
```shell
svn co {{url/to/repository}}
```
#### Bring changes from the repository into the working copy:
```shell
svn up
```
#### Put files and directories under version control, scheduling them for addition to repository. They will be added in next commit:
```shell
svn add {{PATH}}
```
#### Send changes from your working copy to the repository:
```shell
svn ci -m {{commit_log_message}} [{{PATH}}]
```
#### Display changes from the last 10 revisions, showing modified files for each revision:
```shell
svn log -vl {{10}}
```
#### Show detailed help:
```shell
svn help
```
{% endraw %}