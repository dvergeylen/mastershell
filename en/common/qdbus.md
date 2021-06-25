---
layout: default
title: "qdbus"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qdbus">
  <a href="/en/common/qdbus.html">qdbus</a> <a href="#qdbus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inter-Process Communication (IPC) and Remote Procedure Calling (RPC) mechanism originally developed for Linux.
> More information: <https://doc.qt.io/qt-5/qtdbus-index.html>.

#### List available service names:
```shell
qdbus
```
#### List object paths for a specific service:
```shell
qdbus {{service_name}}
```
#### List methods, signals and properties available on a specific object:
```shell
qdbus {{service_name}} {{/path/to/object}}
```
#### Execute a specific method passing arguments and display the returned value:
```shell
qdbus {{service_name}} {{/path/to/object}} {{method_name}} {{argument1}} {{argument2}}
```
#### Display the current brightness value in a KDE Plasma session:
```shell
qdbus {{org.kde.Solid.PowerManagement}} {{/org/kde/Solid/PowerManagement/Actions/BrightnessControl}} {{org.kde.Solid.PowerManagement.Actions.BrightnessControl.brightness}}
```
#### Set a specific brightness to a KDE Plasma session:
```shell
qdbus {{org.kde.Solid.PowerManagement}} {{/org/kde/Solid/PowerManagement/Actions/BrightnessControl}} {{org.kde.Solid.PowerManagement.Actions.BrightnessControl.setBrightness}} {{5000}}
```
#### Invoke volume up shortcut in a KDE Plasma session:
```shell
qdbus {{org.kde.kglobalaccel}} {{/component/kmix}} {{invokeShortcut}} "{{increase_volume}}"
```
#### Display help:
```shell
qdbus --help
```
{% endraw %}