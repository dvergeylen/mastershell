---
layout: default
title: "git root"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-root">
  <a href="/en/common/git-root.html">git root</a> <a href="#git-root"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the root directory of the current Git repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-root>.

#### Print the absolute path of the current Git repository:
```shell
git root
```
#### Print the current working directory relative to the root of the current Git repository:
```shell
git root --relative
```
{% endraw %}