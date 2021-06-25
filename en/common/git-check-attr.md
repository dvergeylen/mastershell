---
layout: default
title: "git check-attr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-check-attr">
  <a href="/en/common/git-check-attr.html">git check-attr</a> <a href="#git-check-attr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> For every pathname, list if each attribute is unspecified, set, or unset as a gitattribute on that pathname.
> More information: <https://git-scm.com/docs/git-check-attr>.

#### Check the values of all attributes on a file:
```shell
git check-attr --all {{path/to/file}}
```
#### Check the value of a specific attribute on a file:
```shell
git check-attr {{attribute}} {{path/to/file}}
```
#### Check the value of a specific attribute on files:
```shell
git check-attr --all {{path/to/file1}} {{path/to/file2}}
```
#### Check the value of a specific attribute on one or more files:
```shell
git check-attr {{attribute}} {{path/to/file1}} {{path/to/file2}}
```
{% endraw %}