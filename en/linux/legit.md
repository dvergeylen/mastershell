---
layout: default
title: "legit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="legit">
  <a href="/en/linux/legit.html">legit</a> <a href="#legit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Complementary command-line interface for Git.
> More information: <https://frostming.github.io/legit>.

#### Switch to a specified branch, stashing and restoring unstaged changes:
```shell
git switch {{target_branch}}
```
#### Synchronize current branch, automatically merging or rebasing, and stashing and unstashing:
```shell
git sync
```
#### Publish a specified branch to the remote server:
```shell
git publish {{branch_name}}
```
#### Remove a branch from the remote server:
```shell
git unpublish {{branch_name}}
```
#### List all branches and their publication status:
```shell
git branches {{glob_pattern}}
```
#### Remove the last commit from the history:
```shell
git undo {{--hard}}
```
{% endraw %}