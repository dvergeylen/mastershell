---
layout: default
title: "git var"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-var">
  <a href="/en/common/git-var.html">git var</a> <a href="#git-var"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints a Git logical variable's value.
> See `git config`, which is preferred over `git var`.
> More information: <https://git-scm.com/docs/git-var>.

#### Print the value of a Git logical variable:
```shell
git var {{GIT_AUTHOR_IDENT|GIT_COMMITTER_IDENT|GIT_EDITOR|GIT_PAGER}}
```
#### [l]ist all Git logical variables:
```shell
git var -l
```
{% endraw %}