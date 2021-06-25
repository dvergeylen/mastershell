---
layout: default
title: "git revert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-revert">
  <a href="/en/common/git-revert.html">git revert</a> <a href="#git-revert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create new commits which reverse the effect of earlier ones.
> More information: <https://git-scm.com/docs/git-revert>.

#### Revert the most recent commit:
```shell
git revert {{@}}
```
#### Revert the 5th last commit:
```shell
git revert HEAD~{{4}}
```
#### Revert multiple commits:
```shell
git revert {{branch_name~5..branch_name~2}}
```
#### Don't create new commits, just change the working tree:
```shell
git revert -n {{0c01a9..9a1743}}
```
{% endraw %}