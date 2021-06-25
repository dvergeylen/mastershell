---
layout: default
title: "git am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-am">
  <a href="/en/common/git-am.html">git am</a> <a href="#git-am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apply patch files. Useful when receiving commits via email.
> See also `git format-patch`, which can generate patch files.
> More information: <https://git-scm.com/docs/git-am>.

#### Apply a patch file:
```shell
git am {{path/to/file.patch}}
```
#### Abort the process of applying a patch file:
```shell
git am --abort
```
#### Apply as much of a patch file as possible, saving failed hunks to reject files:
```shell
git am --reject {{path/to/file.patch}}
```
{% endraw %}