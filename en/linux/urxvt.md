---
layout: default
title: "urxvt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="urxvt">
  <a href="/en/linux/urxvt.html">urxvt</a> <a href="#urxvt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rxvt-unicode.
> A customizable terminal emulator.

#### Open a new urxvt window:
```shell
urxvt
```
#### Run in a specific directory:
```shell
urxvt -cd {{path/to/directory}}
```
#### Run a command in a new urxvt window:
```shell
urxvt -e {{command}}
```
#### Run a command and keep the window open:
```shell
urxvt --hold -e {{command}}
```
#### Run a command within the `sh` shell:
```shell
urxvt -e {{sh}} -c {{command}}
```
{% endraw %}