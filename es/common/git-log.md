---
layout: default
title: "git log"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-log">
  <a href="/es/common/git-log.html">git log</a> <a href="#git-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra un historial de commits.
> Más información: <https://git-scm.com/docs/git-log>.

#### Muestra la secuencia de commits comenzando desde el actual, en orden cronológico inverso, del respositorio de Git en el directorio de trabajo actual:
```shell
git log
```
#### Muestra el historial de un archivo o directorio específico, incluyendo las diferencias:
```shell
git log -p {{ruta/al/archivo_o_directorio}}
```
#### Muestra un resumen de los archivos, o archivo, cambiados en cada commit:
```shell
git log --stat
```
#### Muestra un gráfico de los commits en la rama actual, utilizando solo la primer línea del mensaje de cada uno:
```shell
git log --oneline --graph
```
#### Muestra un gráfico de todos los commits, etiquetas y ramas en todo el repositorio:
```shell
git log --oneline --decorate --all --graph
```
#### Muestra solo los commits cuyo mensaje incluye una cadena dada (no diferencia entre mayúsculas y minúsculas):
```shell
git log -i --grep {{cadena_a_buscar}}
```
#### Muestra los últimos N commits de cierto autor:
```shell
git log -n {{numero}} --author={{autor}}
```
#### Muestra los commits entre dos fechas:
```shell
git log --before={{fecha}} --after={{fecha}}
```
{% endraw %}