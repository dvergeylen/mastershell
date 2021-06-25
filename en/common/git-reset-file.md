---
layout: default
title: "git reset-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reset-file">
  <a href="/en/common/git-reset-file.html">git reset-file</a> <a href="#git-reset-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Revert a file to HEAD or a specific commit.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-reset-file>.

#### Reset a file to HEAD:
```shell
git reset-file {{path/to/file}}
```
#### Reset a file to a specific commit:
```shell
git reset-file {{path/to/file}} {{commit_hash}}
```
{% endraw %}