---
layout: default
title: "git bisect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bisect">
  <a href="/en/common/git-bisect.html">git bisect</a> <a href="#git-bisect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Use binary search to find the commit that introduced a bug.
> Git automatically jumps back and forth in the commit graph to progressively narrow down the faulty commit.
> More information: <https://git-scm.com/docs/git-bisect>.

#### Start a bisect session on a commit range bounded by a known buggy commit, and a known clean (typically older) one:
```shell
git bisect start {{bad_commit}} {{good_commit}}
```
#### For each commit that `git bisect` selects, mark it as "bad" or "good" after testing it for the issue:
```shell
git bisect {{good|bad}}
```
#### After `git bisect` pinpoints the faulty commit, end the bisect session and return to the previous branch:
```shell
git bisect reset
```
#### Skip a commit during a bisect (e.g. one that fails the tests due to a different issue):
```shell
git bisect skip
```
{% endraw %}