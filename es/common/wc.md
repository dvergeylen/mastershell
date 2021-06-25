---
layout: default
title: "wc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wc">
  <a href="/es/common/wc.html">wc</a> <a href="#wc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cuenta líneas, palabras, o bytes.
> Más información: <https://www.gnu.org/software/coreutils/wc>

#### Cuenta las líneas en un archivo:
```shell
wc -l {{ruta/al/archivo}}
```
#### Cuenta las palabras en un archivo:
```shell
wc -w {{ruta/al/archivo}}
```
#### Cuenta caracteres (bytes) en un archivo:
```shell
wc -c {{ruta/al/archivo}}
```
#### Cuenta caracteres en un archivo (considerando los caracteres de varios bytes):
```shell
wc -m {{ruta/al/archivo}}
```
#### Usa la entrada estandar para contar líneas, palabras o caracteres (bytes), en ese orden:
```shell
{{find .}} | wc
```
{% endraw %}