---
layout: default
title: "git cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cp">
  <a href="/en/common/git-cp.html">git cp</a> <a href="#git-cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy an existing file to a new location, preserving history.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-cp>.

#### Copy an existing file in a Git repo, staying in the same directory:
```shell
git cp {{file}} {{new_file}}
```
#### Copy an existing file in a Git repo and place it elsewhere:
```shell
git cp {{path/to/file}} {{path/to/new_file}}
```
{% endraw %}