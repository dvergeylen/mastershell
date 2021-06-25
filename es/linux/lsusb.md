---
layout: default
title: "lsusb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsusb">
  <a href="/es/linux/lsusb.html">lsusb</a> <a href="#lsusb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra información sobre puertos y dispositivos USB.

#### Lista todos los dispositivos USB disponibles:
```shell
lsusb
```
#### Lista la jerarquía de dispositivos USB en forma de árbol:
```shell
lsusb -t
```
#### Lista los dispositivos USB de forma verbosa:
```shell
lsusb --verbose
```
#### Lista información detallada acerca de un dispositivo USB determinado:
```shell
lsusb -D {{dispositivo}}
```
#### Lista solo dispositivos con un ID de ensamblador y producto determinado:
```shell
lsusb -d {{ensamblador}}:{{producto}}
```
{% endraw %}