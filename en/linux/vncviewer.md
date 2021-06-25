---
layout: default
title: "vncviewer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vncviewer">
  <a href="/en/linux/vncviewer.html">vncviewer</a> <a href="#vncviewer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Launches a VNC (Virtual Network Computing) client.

#### Launch a VNC client which connects to a host on a given display:
```shell
vncviewer {{host}}:{{display_number}}
```
#### Launch in full-screen mode:
```shell
vncviewer -FullScreen {{host}}:{{display_number}}
```
#### Launch a VNC client with a specific screen geometry:
```shell
vncviewer --geometry {{width}}x{{height}} {{host}}:{{display_number}}
```
#### Launch a VNC client which connects to a host on a given port:
```shell
vncviewer {{host}}::{{port}}
```
{% endraw %}