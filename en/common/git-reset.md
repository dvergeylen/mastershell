---
layout: default
title: "git reset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reset">
  <a href="/en/common/git-reset.html">git reset</a> <a href="#git-reset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Undo commits or unstage changes, by resetting the current Git HEAD to the specified state.
> If a path is passed, it works as "unstage"; if a commit hash or branch is passed, it works as "uncommit".
> More information: <https://git-scm.com/docs/git-reset>.

#### Unstage everything:
```shell
git reset
```
#### Unstage specific file(s):
```shell
git reset {{path/to/file(s)}}
```
#### Interactively unstage portions of a file:
```shell
git reset --patch {{path/to/file}}
```
#### Undo the last commit, keeping its changes (and any further uncommitted changes) in the filesystem:
```shell
git reset HEAD~
```
#### Undo the last two commits, adding their changes to the index, i.e. staged for commit:
```shell
git reset --soft HEAD~2
```
#### Discard any uncommitted changes, staged or not (for only unstaged changes, use `git checkout`):
```shell
git reset --hard
```
#### Reset the repository to a given commit, discarding committed, staged and uncommitted changes since then:
```shell
git reset --hard {{commit}}
```
{% endraw %}