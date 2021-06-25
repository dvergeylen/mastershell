---
layout: default
title: "git gc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-gc">
  <a href="/en/common/git-gc.html">git gc</a> <a href="#git-gc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimise the local repository by cleaning unnecessary files.
> More information: <https://git-scm.com/docs/git-gc>.

#### Optimise the repository:
```shell
git gc
```
#### Aggressively optimise, takes more time:
```shell
git gc --aggressive
```
#### Do not prune loose objects (prunes by default):
```shell
git gc --no-prune
```
#### Suppress all output:
```shell
git gc --quiet
```
#### View full usage:
```shell
git gc --help
```
{% endraw %}