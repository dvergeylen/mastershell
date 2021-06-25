---
layout: default
title: "xsel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xsel">
  <a href="/en/linux/xsel.html">xsel</a> <a href="#xsel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> X11 selection and clipboard manipulation tool.

#### Use a command's output as input of the clip[b]oard (equivalent to `Ctrl + C`):
```shell
echo 123 | xsel -ib
```
#### Use the contents of a file as input of the clipboard:
```shell
cat {{file}} | xsel -ib
```
#### Output the clipboard's contents into the terminal (equivalent to `Ctrl + V`):
```shell
xsel -ob
```
#### Output the clipboard's contents into a file:
```shell
xsel -ob > {{file}}
```
#### Clear the clipboard:
```shell
xsel -cb
```
#### Output the X11 primary selection's contents into the terminal (equivalent to a mouse middle-click):
```shell
xsel -op
```
{% endraw %}