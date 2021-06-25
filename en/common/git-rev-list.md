---
layout: default
title: "git rev-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-list">
  <a href="/en/common/git-rev-list.html">git rev-list</a> <a href="#git-rev-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List revisions (commits) in reverse chronological order.
> More information: <https://git-scm.com/docs/git-rev-list>.

#### List all commits on the current branch:
```shell
git rev-list {{HEAD}}
```
#### List commits more recent than a specific date, on a specific branch:
```shell
git rev-list --since={{'2019-12-01 00:00:00'}} {{branch_name}}
```
#### List all merge commits on a specific commit:
```shell
git rev-list --merges {{commit}}
```
{% endraw %}