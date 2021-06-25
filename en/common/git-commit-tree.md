---
layout: default
title: "git commit-tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit-tree">
  <a href="/en/common/git-commit-tree.html">git commit-tree</a> <a href="#git-commit-tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Low level utility to create commit objects.
> See also: `git commit`.
> More information: <https://git-scm.com/docs/git-commit-tree>.

#### Create a commit object with the specified message:
```shell
git commit-tree {{tree}} -m "{{message}}"
```
#### Create a commit object reading the message from a file (use `-` for stdin):
```shell
git commit-tree {{tree}} -F {{path/to/file}}
```
#### Create a GPG-signed commit object:
```shell
git commit-tree {{tree}} -m "{{message}}" --gpg-sign
```
#### Create a commit object with the specified parent commit object:
```shell
git commit-tree {{tree}} -m "{{message}}" -p {{parent_commit_sha}}
```
{% endraw %}