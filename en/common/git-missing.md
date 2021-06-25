---
layout: default
title: "git missing"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-missing">
  <a href="/en/common/git-missing.html">git missing</a> <a href="#git-missing"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show commits which aren't shared between two branches.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-missing>.

#### Show commits which aren't shared between the currently checked-out branch and another branch:
```shell
git missing {{branch}}
```
#### Show commits which aren't shared between two branches:
```shell
git missing {{branch_1}} {{branch_2}}
```
{% endraw %}