---
layout: default
title: "most"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="most">
  <a href="/en/common/most.html">most</a> <a href="#most"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open one or several files for interactive reading, allowing scrolling and search.

#### Open a file:
```shell
most {{path/to/file}}
```
#### Open several files:
```shell
most {{path/to/file1}} {{path/to/file2}}
```
#### Open a file at the first occurrence of "string":
```shell
most {{file}} +/{{string}}
```
#### Move through opened files:
```shell
:O n
```
#### Jump to the 100th line:
```shell
{{100}}j
```
#### Edit current file:
```shell
e
```
#### Split the current window in half:
```shell
<CTRL-x> o
```
#### Exit:
```shell
Q
```
{% endraw %}