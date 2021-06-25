---
layout: default
title: "git branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-branch">
  <a href="/en/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Main Git command for working with branches.
> More information: <https://git-scm.com/docs/git-branch>.

#### List local branches. The current branch is highlighted by `*`:
```shell
git branch
```
#### List all branches (local and remote):
```shell
git branch -a
```
#### Show the name of the current branch:
```shell
git branch --show-current
```
#### Create new branch based on the current commit:
```shell
git branch {{branch_name}}
```
#### Create new branch based on a specific commit:
```shell
git branch {{branch_name}} {{commit_hash}}
```
#### Rename a branch (must not have it checked out to do this):
```shell
git branch -m {{old_branch_name}} {{new_branch_name}}
```
#### Delete a local branch (must not have it checked out to do this):
```shell
git branch -d {{branch_name}}
```
#### Delete a remote branch:
```shell
git push {{remote_name}} --delete {{remote_branch_name}}
```
{% endraw %}