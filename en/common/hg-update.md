---
layout: default
title: "hg update"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-update">
  <a href="/en/common/hg-update.html">hg update</a> <a href="#hg-update"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Update the working directory to a specified changeset.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#update>.

#### Update to the tip of the current branch:
```shell
hg update
```
#### Update to the specified revision:
```shell
hg update --rev {{revision}}
```
#### Update and discard uncommitted changes:
```shell
hg update --clean
```
#### Update to the last commit matching a specified date:
```shell
hg update --date {{dd-mm-yyyy}}
```
{% endraw %}