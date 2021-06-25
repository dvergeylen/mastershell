---
layout: default
title: "mdfind"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdfind">
  <a href="/en/osx/mdfind.html">mdfind</a> <a href="#mdfind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List files matching a given query.

#### Find a file by its name:
```shell
mdfind -name {{file}}
```
#### Find a file by its content:
```shell
mdfind {{query}}
```
#### Find a file containing a string, in a given directory:
```shell
mdfind -onlyin {{directory}} {{query}}
```
{% endraw %}