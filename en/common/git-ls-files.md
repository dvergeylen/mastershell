---
layout: default
title: "git ls-files"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-files">
  <a href="/en/common/git-ls-files.html">git ls-files</a> <a href="#git-ls-files"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about files in the index and the working tree.
> More information: <https://git-scm.com/docs/git-ls-files>.

#### Show deleted files:
```shell
git ls-files --deleted
```
#### Show modified and deleted files:
```shell
git ls-files --modified
```
#### Show ignored and untracked files:
```shell
git ls-files --others
```
{% endraw %}