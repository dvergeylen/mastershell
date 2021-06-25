---
layout: default
title: "git delta"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-delta">
  <a href="/en/common/git-delta.html">git delta</a> <a href="#git-delta"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List files that differ from another branch.
> Part of git-extras.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-delta>.

#### List files from the current checked out branch that differ from the `main` branch:
```shell
git delta {{main}}
```
#### List files from specific branch that differ from another specific branch:
```shell
git delta {{branch_1}} {{branch_2}}
```
{% endraw %}