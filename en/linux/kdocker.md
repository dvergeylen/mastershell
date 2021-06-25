---
layout: default
title: "kdocker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kdocker">
  <a href="/en/linux/kdocker.html">kdocker</a> <a href="#kdocker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Easily dock applications to the system tray.
> More information: <https://github.com/user-none/KDocker>.

#### Display a cursor to send a window to the system tray when pressing the left mouse button (press any other mouse button to cancel):
```shell
kdocker
```
#### Open an application and send it to the system tray:
```shell
kdocker {{application}}
```
#### Send focused window to the system tray:
```shell
kdocker -f
```
#### Display a cursor to send a window to the system tray with a custom icon when pressing the left mouse button:
```shell
kdocker -i {{/path/to/icon}}
```
#### Open an application, send it to the system tray and if focus is lost, minimize it:
```shell
kdocker -l {{application}}
```
#### Print version:
```shell
kdocker --version
```
{% endraw %}