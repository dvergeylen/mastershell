---
layout: default
title: "git worktree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-worktree">
  <a href="/en/common/git-worktree.html">git worktree</a> <a href="#git-worktree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage multiple working trees attached to the same repository.
> More information: <https://git-scm.com/docs/git-worktree>.

#### Create a new directory with the specified branch checked out into it:
```shell
git worktree add {{path/to/directory}} {{branch}}
```
#### Create a new directory with a new branch checked out into it:
```shell
git worktree add {{path/to/directory}} -b {{new_branch}}
```
#### List all the working directories attached to this repository:
```shell
git worktree list
```
#### Remove a worktree (after deleting worktree directory):
```shell
git worktree prune
```
{% endraw %}