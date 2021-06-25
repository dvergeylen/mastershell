---
layout: default
title: "mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mv">
  <a href="/es/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mueve o renombra archivos y directorios.
> Más información: <https://www.gnu.org/software/coreutils/mv>.

#### Mueve archivos en ubicaciones arbitrarias:
```shell
mv {{origen}} {{destino}}
```
#### Mueve sin solicitar confirmación antes de sobrescribir archivos existentes:
```shell
mv -f {{origen}} {{destino}}
```
#### Solicita confirmación antes de sobrescribir archivos existentes, independientemente de los permisos del archivo:
```shell
mv -i {{origen}} {{destino}}
```
#### No sobrescribe archivos existentes en el destino:
```shell
mv -n {{origen}} {{destino}}
```
#### Mueve archivos en modo detallado, mostrando los archivos después de moverlos:
```shell
mv -v {{origen}} {{destino}}
```
{% endraw %}