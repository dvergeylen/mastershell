---
layout: default
title: "git switch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-switch">
  <a href="/en/common/git-switch.html">git switch</a> <a href="#git-switch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Switch between Git branches. Requires Git version 2.23+.
> See also `git checkout`.
> More information: <https://git-scm.com/docs/git-switch>.

#### Switch to an existing branch:
```shell
git switch {{branch_name}}
```
#### Create a new branch and switch to it:
```shell
git switch --create {{branch_name}}
```
#### Create a new branch based on an existing commit and switch to it:
```shell
git switch --create {{branch_name}} {{commit}}
```
#### Switch to the previous branch:
```shell
git switch -
```
#### Switch to a branch and update all submodules to match:
```shell
git switch --recurse-submodules {{branch_name}}
```
#### Switch to a branch and automatically merge the current branch and any uncommitted changes into it:
```shell
git switch --merge {{branch_name}}
```
{% endraw %}