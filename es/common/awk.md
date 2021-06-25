---
layout: default
title: "awk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="awk">
  <a href="/es/common/awk.html">awk</a> <a href="#awk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un lenguaje de programación versátil para trabajar con archivos.
> Más información: <https://github.com/onetrueawk/awk>.

#### Imprime la quinta columna (también conocido como campo) en un archivo separado por espacios:
```shell
awk '{print $5}' {{archivo}}
```
#### Imprime la segunda columna de las líneas que contengan "algo" en un archivo separado por espacios:
```shell
awk '/{{algo}}/ {print $2}' {{archivo}}
```
#### Imprime la última columna de cada línea de un archivo, usando la coma (en vez de espacio) como separador de campo:
```shell
awk -F ',' '{print $NF}' {{archivo}}
```
#### Suma los valores en de la primera columna de un archivo e imprime el total:
```shell
awk '{s+=$1} END {print s}' {{archivo}}
```
#### Suma los valores en de la primera columna de un archivo e imprime el total de froma bonita:
```shell
awk '{s+=$1; print $1} END {print "--------"; print s}' {{archivo}}
```
#### Imprime cada tres líneas, empezando por la primera:
```shell
awk 'NR%3==1' {{archivo}}
```
#### Imprime todos los valores desde la tercera columna:
```shell
awk '{for (i=3; i <= NF; i++) printf $i""FS; print""}' {{archivo}}
```
#### Imprime diferentes valores dependiendo de condiciones:
```shell
awk '{if ($1 == "foo") print "Coincidencia completa foo"; else if ($1 ~ "bar") print "Coincidencia parcial bar"; else print "Baz"}' {{archivo}}
```
{% endraw %}