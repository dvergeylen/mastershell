---
layout: default
title: "hg log"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-log">
  <a href="/en/common/hg-log.html">hg log</a> <a href="#hg-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the revision history of the repository.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#log>.

#### Display the entire revision history of the repository:
```shell
hg log
```
#### Display the revision history with an ASCII graph:
```shell
hg log --graph
```
#### Display the revision history with file names matching a specified pattern:
```shell
hg log --include {{pattern}}
```
#### Display the revision history, excluding file names that match a specified pattern:
```shell
hg log --exclude {{pattern}}
```
#### Display the log information for a specific revision:
```shell
hg log --rev {{revision}}
```
#### Display the revision history for a specific branch:
```shell
hg log --branch {{branch}}
```
#### Display the revision history for a specific date:
```shell
hg log --date {{date}}
```
#### Display revisions committed by a specific user:
```shell
hg log --user {{user}}
```
{% endraw %}