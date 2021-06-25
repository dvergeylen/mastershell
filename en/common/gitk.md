---
layout: default
title: "gitk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gitk">
  <a href="/en/common/gitk.html">gitk</a> <a href="#gitk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A graphical Git repository browser.
> More information: <https://git-scm.com/docs/gitk>.

#### Show the repository browser for the current Git repository:
```shell
gitk
```
#### Show repository browser for a specific file or directory:
```shell
gitk {{path/to/file_or_directory}}
```
#### Show commits made since 1 week ago:
```shell
gitk --since="{{1 week ago}}"
```
#### Show commits older than 1/1/2016:
```shell
gitk --until="{{1/1/2015}}"
```
#### Show at most 100 changes in all branches:
```shell
 gitk --max-count={{100}} --all
```
{% endraw %}