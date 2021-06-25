---
layout: default
title: "git svn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-svn">
  <a href="/en/common/git-svn.html">git svn</a> <a href="#git-svn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bidirectional operation between a Subversion repository and Git.
> More information: <https://git-scm.com/docs/git-svn>.

#### Clone an SVN repository:
```shell
git svn clone {{https://example.com/subversion_repo}} {{local_dir}}
```
#### Clone a SVN repository starting at a given revision number:
```shell
git svn clone -r{{1234}}:HEAD {{https://svn.example.net/subversion/repo}} {{local_dir}}
```
#### Update local clone from the remote SVN repository:
```shell
git svn rebase
```
#### Fetch updates from the remote SVN repository without changing the Git HEAD:
```shell
git svn fetch
```
#### Commit back to the SVN repository:
```shell
git svn dcommit
```
{% endraw %}