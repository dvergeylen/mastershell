---
layout: default
title: "vncserver"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vncserver">
  <a href="/en/linux/vncserver.html">vncserver</a> <a href="#vncserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Launches a VNC (Virtual Network Computing) desktop.

#### Launch a VNC Server on next available display:
```shell
vncserver
```
#### Launch a VNC Server with specific screen geometry:
```shell
vncserver --geometry {{width}}x{{height}}
```
#### Kill an instance of VNC Server running on a specific display:
```shell
vncserver --kill :{{display_number}}
```
{% endraw %}