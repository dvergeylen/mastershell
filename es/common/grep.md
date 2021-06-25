---
layout: default
title: "grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grep">
  <a href="/es/common/grep.html">grep</a> <a href="#grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encuentra coincidencias en el texto introducido.
> Soporta patrones simples y expresiones regulares.
> Más información: <https://www.gnu.org/software/grep/manual/grep.html>

#### Busca un patrón dentro de un archivo:
```shell
grep {{patron}} {{ruta/al/archivo}}
```
#### Busca un patrón exacto:
```shell
grep -F {{patron_exacto}} {{ruta/al/archivo}}
```
#### Busca un patrón [R]ecursivamente en el directorio actual, mostrando los correspondientes [n]úmeros de línea, [I]gnorando archivos binarios:
```shell
grep -RIn {{patron}} .
```
#### Usa expresiones regulares extendidas (soportando `?`, `+`, `{}`, `()` y `|`), sin importar mayúsculas o minúsculas:
```shell
grep -Ei {{patron}} {{ruta/al/archivo}}
```
#### Imprime 3 líneas de [C]ontexto alrededor, anteriores ([B]), o posteriores ([A]) tras la coincidencia:
```shell
grep -{{C|B|A}} 3 {{patron}} {{ruta/al/archivo}}
```
#### Imprime el nombre del archivo con la línea correspondiente a cada coincidencia:
```shell
grep -Hn {{patron}} {{ruta/al/archivo}}
```
#### Usa la entrada estándar en vez de un archivo:
```shell
cat {{ruta/al/archivo}} | grep {{patron}}
```
#### Encuentra coincidencias in[v]ersas al patrón (aquellas líneas que no lo contengan):
```shell
grep -v {{patron}}
```
{% endraw %}