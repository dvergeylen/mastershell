---
layout: default
title: "clamav"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clamav">
  <a href="/es/linux/clamav.html">clamav</a> <a href="#clamav"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Antivirus de código abierto.
> Diseñado especialment para escanear correos electrónicos, pero puede ser usado en otros contextos.
> Más información: <https://www.clamav.net>.

#### Actualiza definiciones de virus:
```shell
freshclam
```
#### Escanea un archivo en busca de virus:
```shell
clamscan {{ruta/al/archivo}}
```
#### Escanea directorios recursivamente y mostrar los archivos infectados:
```shell
clamscan --recursive --infected {{ruta/al/directorio}}
```
#### Escanea directorios recursivamente y poner los archivos infectados en cuarentena:
```shell
clamscan --recursive --move={{directorio}}
```
{% endraw %}