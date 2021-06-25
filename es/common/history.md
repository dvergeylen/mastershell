---
layout: default
title: "history"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="history">
  <a href="/es/common/history.html">history</a> <a href="#history"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Historial de la línea de comandos.
> Más información: <https://www.gnu.org/software/bash/manual/html_node/Bash-History-Builtins.html>.

#### Muestra el historial de comandos junto a su número de línea:
```shell
history
```
#### Muestra los últimos 20 comandos:
```shell
history {{20}}
```
#### Limpia el historial de comandos (solo para la shell actual):
```shell
history -c
```
#### Sobrescribe el archivo histórico con el historial de la shell actual (comúnmente se combina con `history -c` para limpiar el historial):
```shell
history -w
```
#### Borra la entrada del historial en el índice especificado:
```shell
history -d {{indice}}
```
{% endraw %}