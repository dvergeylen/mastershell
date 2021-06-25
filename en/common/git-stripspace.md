---
layout: default
title: "git stripspace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stripspace">
  <a href="/en/common/git-stripspace.html">git stripspace</a> <a href="#git-stripspace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read text (e.g. commit messages, notes, tags, and branch descriptions) from the standard input and clean it into the manner used by Git.
> More information: <https://git-scm.com/docs/git-stripspace>.

#### Trim whitespace from a file:
```shell
cat {{path/to/file}} | git stripspace
```
#### Trim whitespace and Git comments from a file:
```shell
cat {{path/to/file}} | git stripspace --strip-comments
```
#### Convert all lines in a file into Git comments:
```shell
git stripspace --comment-lines < {{path/to/file}}
```
{% endraw %}