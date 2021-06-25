---
layout: default
title: "aapt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aapt">
  <a href="/es/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para empaquetado de activos de Android.
> Compila y empaqueta recursos de una app de Android.
> Más información: <https://elinux.org/Android_aapt>.

#### Lista los archivos contenidos en un archivo APK:
```shell
aapt list {{ruta/al/app.apk}}
```
#### Muestra la metadata de una app (versión, permisos, etc.):
```shell
aapt dump badging {{ruta/al/app.apk}}
```
#### Crea un nuevo archivo APK con archivos de un directorio especificado:
```shell
aapt package -F {{ruta/al/app.apk}} {{ruta/al/directorio}}
```
{% endraw %}