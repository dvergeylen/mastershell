---
layout: default
title: "cmus"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmus">
  <a href="/en/linux/cmus.html">cmus</a> <a href="#cmus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line Music Player.
> Use arrow keys to navigate, `<enter/return>` to select, and numbers 1-8 switch between different views.

#### Open cmus into the specified directory (this will become your new working directory):
```shell
cmus {{path/to/directory}}
```
#### Add file/directory to library:
```shell
:add {{path/to/file_or_directory}}
```
#### Pause/unpause current song:
```shell
c
```
#### Toggle shuffle mode on/off:
```shell
s
```
#### Quit cmus:
```shell
q
```
{% endraw %}