---
layout: default
title: "rig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rig">
  <a href="/es/linux/rig.html">rig</a> <a href="#rig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilidad para generar un nombre, apellido, calle y número, junto a ubicación geográfica consistente (un conjunto válido de ciudad, estado y código postal).
> Más información: <https://manpages.ubuntu.com/manpages/focal/man6/rig.6.html>.

#### Muestra un nombre aleatorio (masculino o femenino) y una dirección:
```shell
rig
```
#### Muestra un nombre [m]asculino, (o [f]emenino) aleatorio y una dirección:
```shell
rig -{{m|f}}
```
#### Usa archivos de datos de un directorio específico (por defecto es `/usr/share/rig`):
```shell
rig -d {{ruta/al/directorio}}
```
#### Especifica el número de identidades a generar:
```shell
rig -c {{numero}}
```
#### Especifica el número de identidades femininas a generar:
```shell
rig -f -c {{numero}}
```
{% endraw %}