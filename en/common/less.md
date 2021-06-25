---
layout: default
title: "less"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="less">
  <a href="/en/common/less.html">less</a> <a href="#less"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open a file for interactive reading, allowing scrolling and search.
> More information: <https://greenwoodsoftware.com/less/>.

#### Open a file:
```shell
less {{source_file}}
```
#### Page down / up:
```shell
<Space> (down), b (up)
```
#### Go to end / start of file:
```shell
G (end), g (start)
```
#### Forward search for a string (press `n`/`N` to go to next/previous match):
```shell
/{{something}}
```
#### Backward search for a string (press `n`/`N` to go to next/previous match):
```shell
?{{something}}
```
#### Follow the output of the currently opened file:
```shell
F
```
#### Open the current file in an editor:
```shell
v
```
#### Exit:
```shell
q
```
{% endraw %}