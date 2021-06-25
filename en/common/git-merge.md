---
layout: default
title: "git merge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-merge">
  <a href="/en/common/git-merge.html">git merge</a> <a href="#git-merge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Merge branches.
> More information: <https://git-scm.com/docs/git-merge>.

#### Merge a branch into your current branch:
```shell
git merge {{branch_name}}
```
#### Edit the merge message:
```shell
git merge -e {{branch_name}}
```
#### Merge a branch and create a merge commit:
```shell
git merge --no-ff {{branch_name}}
```
#### Abort a merge in case of conflicts:
```shell
git merge --abort
```
{% endraw %}