---
layout: default
title: "git create-branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-create-branch">
  <a href="/en/common/git-create-branch.html">git create-branch</a> <a href="#git-create-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a Git branch in a repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-create-branch>.

#### Create a local branch:
```shell
git create-branch {{branch_name}}
```
#### Create a branch locally and on origin:
```shell
git create-branch --remote {{branch_name}}
```
#### Create a branch locally and on upstream (through forks):
```shell
git create-branch --remote upstream {{branch_name}}
```
{% endraw %}