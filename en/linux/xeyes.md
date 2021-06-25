---
layout: default
title: "xeyes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xeyes">
  <a href="/en/linux/xeyes.html">xeyes</a> <a href="#xeyes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display eyes on the screen that follow the mouse cursor.

#### Launch xeyes on the local machine's default display:
```shell
xeyes
```
#### Launch xeyes on a remote machine's display 0, screen 0:
```shell
xeyes -display {{remote_host}}:{{0}}.{{0}}
```
{% endraw %}