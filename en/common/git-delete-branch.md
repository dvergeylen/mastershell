---
layout: default
title: "git delete-branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-delete-branch">
  <a href="/en/common/git-delete-branch.html">git delete-branch</a> <a href="#git-delete-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete local and remote Git branches.
> Part of `git-extras`. If deleting the checked out branch, only the remote branch will be deleted.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-delete-branch>.

#### Delete a local and remote Git branch:
```shell
git delete-branch {{branch_name}}
```
#### Delete multiple local and remote Git branches:
```shell
git delete-branch {{branch_name1 branch_name2 ...}}
```
{% endraw %}