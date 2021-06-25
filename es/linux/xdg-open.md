---
layout: default
title: "xdg-open"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xdg-open">
  <a href="/es/linux/xdg-open.html">xdg-open</a> <a href="#xdg-open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Abre un archivo o URL en la aplicación predeterminada del usuario.
> Más información: <https://man.archlinux.org/man/xdg-open.1>.

#### Abre el directorio actual en el explorador de archivos predeterminado:
```shell
xdg-open .
```
#### Abre una URL en el navegador predeterminado:
```shell
xdg-open {{https://www.ejemplo.es}}
```
#### Abre una image en el visor de imágenes predeterminado:
```shell
xdg-open {{ruta/al/imagen}}
```
#### Abre un PDF en el visor de PDF predeterminado:
```shell
xdg-open {{ruta/al/pdf}}
```
#### Muestra la ayuda:
```shell
xdg-open --help
```
{% endraw %}