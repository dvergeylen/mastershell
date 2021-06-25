---
layout: default
title: "bash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bash">
  <a href="/es/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> Intérprete de línea de comandos compatible con `sh`.
> Más información: <https://gnu.org/software/bash>.

#### Inicia un intérprete de comandos interactivo:
```shell
bash
```
#### Ejecuta un comando:
```shell
bash -c "{{comando}}"
```
#### Ejecuta comandos desde un archivo:
```shell
bash {{archivo.sh}}
```
#### Ejecuta comandos desde un archivo, mostrando todos los comando ejecutados en la terminal:
```shell
bash -x {{archivo.sh}}
```
#### Ejecuta comandos desde un archivo, deteniéndose en el primer error:
```shell
bash -e {{archivo.sh}}
```
#### Ejecuta comandos desde stdin (entrada estándar):
```shell
bash -s
```
#### Imprime la información de la versión de bash (use `echo $BASH_VERSION` para ver sólo la versión sin la información sobre la licencia):
```shell
bash --version
```
{% endraw %}