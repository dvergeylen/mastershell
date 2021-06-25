---
layout: default
title: "git whatchanged"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-whatchanged">
  <a href="/en/common/git-whatchanged.html">git whatchanged</a> <a href="#git-whatchanged"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show what has changed with recent commits or files.
> See also `git log`.
> More information: <https://git-scm.com/docs/git-whatchanged>.

#### Display logs and changes for recent commits:
```shell
git whatchanged
```
#### Display logs and changes for recent commits within the specified time frame:
```shell
git whatchanged --since="{{2 hours ago}}"
```
#### Display logs and changes for recent commits for specific files or directories:
```shell
git whatchanged {{path/to/file_or_directory}}
```
{% endraw %}