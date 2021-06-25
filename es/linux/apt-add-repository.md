---
layout: default
title: "apt-add-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-add-repository">
  <a href="/es/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona las definiciones del repositorio apt.
> Más información: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Añade un nuevo repositorio apt:
```shell
apt-add-repository {{repositorio}}
```
#### Elimina un repositorio apt:
```shell
apt-add-repository --remove {{repositorio}}
```
#### Actualiza la caché de paquetes tras añadir un repositorio:
```shell
apt-add-repository --update {{repositorio}}
```
#### Activar las fuentes de paquetes:
```shell
apt-add-repository --enable-source {{repositorio}}
```
{% endraw %}