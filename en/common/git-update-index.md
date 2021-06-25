---
layout: default
title: "git update-index"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-update-index">
  <a href="/en/common/git-update-index.html">git update-index</a> <a href="#git-update-index"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Git command for manipulating the index.
> More information: <https://git-scm.com/docs/git-update-index>.

#### Pretend that a modified file is unchanged (`git status` will not show this as changed):
```shell
git update-index --skip-worktree {{path/to/modified_file}}
```
{% endraw %}