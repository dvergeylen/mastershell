---
layout: default
title: "git stash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stash">
  <a href="/en/common/git-stash.html">git stash</a> <a href="#git-stash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stash local Git changes in a temporary area.
> More information: <https://git-scm.com/docs/git-stash>.

#### Stash current changes, except new (untracked) files:
```shell
git stash [push -m {{optional_stash_message}}]
```
#### Stash current changes, including new (untracked) files:
```shell
git stash -u
```
#### Interactively select parts of changed files for stashing:
```shell
git stash -p
```
#### List all stashes (shows stash name, related branch and message):
```shell
git stash list
```
#### Apply a stash (default is the latest, named stash@{0}):
```shell
git stash apply {{optional_stash_name_or_commit}}
```
#### Apply a stash (default is stash@{0}), and remove it from the stash list if applying doesn't cause conflicts:
```shell
git stash pop {{optional_stash_name}}
```
#### Drop a stash (default is stash@{0}):
```shell
git stash drop {{optional_stash_name}}
```
#### Drop all stashes:
```shell
git stash clear
```
{% endraw %}