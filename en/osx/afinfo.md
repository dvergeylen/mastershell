---
layout: default
title: "afinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="afinfo">
  <a href="/en/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Audio file metadata parser for OS X.
> Built-in command of OS X.

#### Display info of a given audio file:
```shell
afinfo {{path/to/file}}
```
#### Print a one line description of the audio file:
```shell
afinfo -b {{path/to/file}}
```
#### Print metadata info and contents of the audio file's InfoDictionary:
```shell
afinfo -i {{path/to/file}}
```
#### Print output in xml format:
```shell
afinfo -x {{path/to/file}}
```
#### Print warnings for the audio file if any:
```shell
afinfo --warnings {{path/to/file}}
```
#### Display help for full usage:
```shell
afinfo -h
```
{% endraw %}