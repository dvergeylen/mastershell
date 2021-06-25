---
layout: default
title: "x11docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="x11docker">
  <a href="/en/common/x11docker.html">x11docker</a> <a href="#x11docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Securely run GUI applications and desktop UIs in Docker containers.
> See also `xephyr`.
> More information: <https://github.com/mviereck/x11docker>.

#### Launch VLC in a container:
```shell
x11docker --pulseaudio --share={{$HOME/Videos}} {{jess/vlc}}
```
#### Launch Xfce in a window:
```shell
x11docker --desktop {{x11docker/xfce}}
```
#### Launch GNOME in a window:
```shell
x11docker --desktop --gpu --init={{systemd}} {{x11docker/gnome}}
```
#### Launch KDE Plasma in a window:
```shell
x11docker --desktop --gpu --init={{systemd}} {{x11docker/kde-plasma}}
```
#### Display help:
```shell
x11docker --help
```
{% endraw %}