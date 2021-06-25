---
layout: default
title: "open"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="open">
  <a href="/en/osx/open.html">open</a> <a href="#open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opens files, directories and applications.

#### Open a file with the associated application:
```shell
open {{file.ext}}
```
#### Run a graphical macOS application:
```shell
open -a {{Application}}
```
#### Run a graphical macOS app based on the bundle identifier (refer to `osascript` for an easy way to get this):
```shell
open -b {{com.domain.application}}
```
#### Open the current directory in Finder:
```shell
open .
```
#### Reveal a file in Finder:
```shell
open -R {{path/to/file}}
```
#### Open all the files of a given extension in the current directory with the associated application:
```shell
open {{*.ext}}
```
{% endraw %}