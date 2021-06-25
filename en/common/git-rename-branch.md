---
layout: default
title: "git rename-branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rename-branch">
  <a href="/en/common/git-rename-branch.html">git rename-branch</a> <a href="#git-rename-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename a Git branch.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-rename-branch>.

#### Rename the branch you are currently on:
```shell
git rename-branch {{new_branch_name}}
```
#### Rename a specific branch:
```shell
git rename-branch {{old_branch_name}} {{new_branch_name}}
```
{% endraw %}