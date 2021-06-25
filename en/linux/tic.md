---
layout: default
title: "tic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tic">
  <a href="/en/linux/tic.html">tic</a> <a href="#tic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile terminfo and install for ncurses.
> More information: <https://pubs.opengroup.org/onlinepubs/007908799/xcurses/terminfo.html>.

#### Compile and install terminfo for a terminal:
```shell
tic -xe {{terminal}} {{path/to/terminal.info}}
```
#### Check terminfo file for errors:
```shell
tic -c {{path/to/terminal.info}}
```
#### Print database locations:
```shell
tic -D
```
{% endraw %}