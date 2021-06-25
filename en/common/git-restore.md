---
layout: default
title: "git restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-restore">
  <a href="/en/common/git-restore.html">git restore</a> <a href="#git-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restore working tree files. Requires Git version 2.23+.
> See also `git checkout` and `git reset`.
> More information: <https://git-scm.com/docs/git-restore>.

#### Restore an unstaged file to the version of the current commit (HEAD):
```shell
git restore {{path/to/file}}
```
#### Restore an unstaged file to the version of a specific commit:
```shell
git restore --source {{commit}} {{path/to/file}}
```
#### Discard all unstaged changes to tracked files:
```shell
git restore :/
```
#### Unstage a file:
```shell
git restore --staged {{path/to/file}}
```
#### Unstage all files:
```shell
git restore --staged :/
```
#### Discard all changes to files, both staged and unstaged:
```shell
git restore --worktree --staged :/
```
#### Interactively select sections of files to restore:
```shell
git restore --patch
```
{% endraw %}