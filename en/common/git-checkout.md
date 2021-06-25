---
layout: default
title: "git checkout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-checkout">
  <a href="/en/common/git-checkout.html">git checkout</a> <a href="#git-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checkout a branch or paths to the working tree.
> More information: <https://git-scm.com/docs/git-checkout>.

#### Create and switch to a new branch:
```shell
git checkout -b {{branch_name}}
```
#### Create and switch to a new branch based on a specific reference (branch, remote/branch, tag are examples of valid references):
```shell
git checkout -b {{branch_name}} {{reference}}
```
#### Switch to an existing local branch:
```shell
git checkout {{branch_name}}
```
#### Switch to the previously checked out branch:
```shell
git checkout -
```
#### Switch to an existing remote branch:
```shell
git checkout --track {{remote_name}}/{{branch_name}}
```
#### Discard all unstaged changes in the current directory (see `git reset` for more undo-like commands):
```shell
git checkout .
```
#### Discard unstaged changes to a given file:
```shell
git checkout {{filename}}
```
#### Replace a file in the current directory with the version of it committed in a given branch:
```shell
git checkout {{branch_name}} -- {{filename}}
```
{% endraw %}