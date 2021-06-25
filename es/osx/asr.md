---
layout: default
title: "asr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asr">
  <a href="/es/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restaura (copia) una imagen de disco en un volumen.
> El nombre del comando significa Restauración de Software de Apple.

#### Restaura una imagen de disco en un volumen:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}}
```
#### Borra el volumen deseado antes de restaurar:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}} --erase
```
#### Omite la verificación después de restaurar:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}} --noverify
```
#### Clona volúmenes sin el uso de una imagen de disco intermedia:
```shell
sudo asr restore --source {{ruta/al/volumen}} --target {{ruta/al/volumen_clonado}}
```
{% endraw %}