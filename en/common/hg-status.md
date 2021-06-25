---
layout: default
title: "hg status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-status">
  <a href="/en/common/hg-status.html">hg status</a> <a href="#hg-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show files that have changed in the working directory.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#status>.

#### Display the status of changed files:
```shell
hg status
```
#### Display only modified files:
```shell
hg status --modified
```
#### Display only added files:
```shell
hg status --added
```
#### Display only removed files:
```shell
hg status --removed
```
#### Display only deleted (but tracked) files:
```shell
hg status --deleted
```
#### Display changes in the working directory compared to a specified changeset:
```shell
hg status --rev {{revision}}
```
#### Display only files matching a specified glob pattern:
```shell
hg status --include {{pattern}}
```
#### Display files, excluding those that match a specified glob pattern:
```shell
hg status --exclude {{pattern}}
```
{% endraw %}