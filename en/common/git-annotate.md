---
layout: default
title: "git annotate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-annotate">
  <a href="/en/common/git-annotate.html">git annotate</a> <a href="#git-annotate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show commit hash and last author on each line of a file.
> See `git blame`, which is preferred over `git annotate`.
> `git annotate` is provided for those familiar with other version control systems.
> More information: <https://git-scm.com/docs/git-annotate>.

#### Print a file with the author name and commit hash prepended to each line:
```shell
git annotate {{path/to/file}}
```
#### Print a file with the author email and commit hash prepended to each line:
```shell
git annotate -e {{path/to/file}}
```
{% endraw %}