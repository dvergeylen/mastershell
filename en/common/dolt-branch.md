---
layout: default
title: "dolt branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dolt-branch">
  <a href="/en/common/dolt-branch.html">dolt branch</a> <a href="#dolt-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Dolt branches.
> More information: <https://github.com/dolthub/dolt>.

#### List local branches (current branch is highlighted by `*`):
```shell
dolt branch
```
#### List all local and remote branches:
```shell
dolt branch --all
```
#### Create a new branch based on the current branch:
```shell
dolt branch {{branch_name}}
```
#### Create a new branch with the specified commit as the latest:
```shell
dolt branch {{branch_name}} {{commit}}
```
#### Rename a branch:
```shell
dolt branch --move {{branch_name1}} {{branch_name2}}
```
#### Duplicate a branch:
```shell
dolt branch --copy {{branch_name1}} {{branch_name2}}
```
#### Delete a branch:
```shell
dolt branch --delete {{branch_name}}
```
#### Display the name of the current branch:
```shell
dolt branch --show-current
```
{% endraw %}