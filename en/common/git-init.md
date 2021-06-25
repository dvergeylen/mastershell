---
layout: default
title: "git init"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-init">
  <a href="/en/common/git-init.html">git init</a> <a href="#git-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Initializes a new local Git repository.
> More information: <https://git-scm.com/docs/git-init>.

#### Initialize a new local repository:
```shell
git init
```
#### Initialize a repository with the specified name for the initial branch:
```shell
git init --initial-branch={{branch_name}}
```
#### Initialize a repository using SHA256 for object hashes (requires Git version 2.29+):
```shell
git init --object-format={{sha256}}
```
#### Initialize a barebones repository, suitable for use as a remote over ssh:
```shell
git init --bare
```
{% endraw %}