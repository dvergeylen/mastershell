---
layout: default
title: "git check-ignore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-check-ignore">
  <a href="/es/common/git-check-ignore.html">git check-ignore</a> <a href="#git-check-ignore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analiza y depura los archivos que Git debe ignorar / excluir (.gitignore).
> Más información: <https://git-scm.com/docs/git-check-ignore>.

#### Comprueba si un archivo o directorio es ignorado:
```shell
git check-ignore {{ruta/al/archivo_o_directorio}}
```
#### Comprueba si varios archivos o directorios son ignorados:
```shell
git check-ignore {{ruta/al/archivo}} {{ruta/al/directorio}}
```
#### Usa nombres de rutas, uno por línea, a partir de la entrada estandar (stdin):
```shell
git check-ignore --stdin < {{ruta/al/archivo_lista}}
```
#### No comprueba el índice (se utiliza para depurar por qué las rutas fueron rastreadas y no ignoradas):
```shell
git check-ignore --no-index {{ruta/de_los/archivos_o_directorios}}
```
#### Incluye detalles sobre el patrón de coincidencia para cada ruta:
```shell
git check-ignore --verbose {{ruta/de_los/archivos_o_directorios}}
```
{% endraw %}