---
layout: default
title: "x11vnc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="x11vnc">
  <a href="/en/linux/x11vnc.html">x11vnc</a> <a href="#x11vnc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A VNC server that will enable VNC on an existing display server.
> By default, the server will automatically terminate once all clients disconnect from it.

#### Launch a VNC server that allows multiple clients to connect:
```shell
x11vnc -shared
```
#### Launch a VNC server in view-only mode, and which won't terminate once the last client disconnects:
```shell
x11vnc -forever -viewonly
```
#### Launch a VNC server on a specific display and screen (both starting at index zero):
```shell
x11vnc -display :{{display}}.{{screen}}
```
#### Launch a VNC server on the third display's default screen:
```shell
x11vnc -display :{{2}}
```
#### Launch a VNC server on the first display's second screen:
```shell
x11vnc -display :{{0}}.{{1}}
```
{% endraw %}