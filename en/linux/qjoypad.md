---
layout: default
title: "qjoypad"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qjoypad">
  <a href="/en/linux/qjoypad.html">qjoypad</a> <a href="#qjoypad"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Translate input from gamepads or joysticks into keyboard strokes or mouse actions.
> More information: <http://qjoypad.sourceforge.net/>.

#### Start QJoyPad:
```shell
qjoypad
```
#### Start QJoyPad and look for devices in a specific directory:
```shell
qjoypad --device={{path/to/directory}}
```
#### Start QJoyPad but don't show a system tray icon:
```shell
qjoypad --notray
```
#### Start QJoyPad and force the window manager to use a system tray icon:
```shell
qjoypad --force-tray
```
#### Force a running instance of QJoyPad to update its list of devices and layouts:
```shell
qjoypad --update
```
#### Load the given layout in an already running instance of QJoyPad, or start QJoyPad using the given layout:
```shell
qjoypad "{{layout}}"
```
{% endraw %}