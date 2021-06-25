---
layout: default
title: "cut"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cut">
  <a href="/es/common/cut.html">cut</a> <a href="#cut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recorta campos provenientes de la entrada estándar o de archivos.
> Más información: <https://www.gnu.org/software/coreutils/cut>

#### Recorta los primeros 16 caracteres de cada línea de la entrada estándar:
```shell
cut -c {{1-16}}
```
#### Recorta los primeros 16 caracteres de cada línea de los archivos especificados:
```shell
cut -c {{1-16}} {{archivo}}
```
#### Recorta todo desde el tercer caracter hasta el final de cada línea:
```shell
cut -c {{3-}}
```
#### Recorta el quinto campo de cada línea, usando los dos puntos como delimitadores de campos (por defecto el delimitador es tab):
```shell
cut -d'{{:}}' -f{{5}}
```
#### Recorta el segundo y décimo campo de cada línea, usando los punto y coma como delimitadores:
```shell
cut -d'{{;}}' -f{{2,10}}
```
#### Recorta los campos del tercero al último de cada línea, usando los espacios como delimintadores:
```shell
cut -d'{{ }}' -f{{3-}}
```
{% endraw %}