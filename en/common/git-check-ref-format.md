---
layout: default
title: "git check-ref-format"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-check-ref-format">
  <a href="/en/common/git-check-ref-format.html">git check-ref-format</a> <a href="#git-check-ref-format"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checks if a given refname is acceptable, and exits with a non-zero status if it is not.
> More information: <https://git-scm.com/docs/git-check-ref-format>.

#### Check the format of the specified refname:
```shell
git check-ref-format {{refs/head/refname}}
```
#### Print the name of the last branch checked out:
```shell
git check-ref-format --branch @{-1}
```
#### Normalize a refname:
```shell
git check-ref-format --normalize {{refs/head/refname}}
```
{% endraw %}