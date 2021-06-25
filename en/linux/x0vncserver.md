---
layout: default
title: "x0vncserver"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="x0vncserver">
  <a href="/en/linux/x0vncserver.html">x0vncserver</a> <a href="#x0vncserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> TigerVNC Server for X displays.
> More information: <https://tigervnc.org/doc/x0vncserver.html>.

#### Start a VNC server using a passwordfile:
```shell
x0vncserver -display {{:0}} -passwordfile {{path/to/file}}
```
#### Start a VNC server using a specific port:
```shell
x0vncserver -display {{:0}} -rfbport {{port}}
```
{% endraw %}