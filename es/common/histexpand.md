---
layout: default
title: "history expansion"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="history-expansion">
  <a href="/es/common/histexpand.html">history expansion</a> <a href="#history-expansion"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reutiliza y expande el historial de la shell en `sh`, `bash`, `zsh`, `rbash` y `ksh`.
> Más información: <https://www.gnu.org/software/bash/manual/html_node/History-Interaction>.

#### Ejecuta el último comando:
```shell
!!
```
#### Ejecuta el último comando como administrador:
```shell
sudo !!
```
#### Ejecuta un comando con el último argumento del último comando:
```shell
{{comando}} !$
```
#### Ejecuta un comando con el primer argumento del comando anterior:
```shell
{{comando}} !^
```
#### Ejecuta el comando `n` líneas atrás en el historial:
```shell
!-{{n}}
```
#### Ejecuta el último comando con el prefijo `cadena`:
```shell
!{{cadena}}
```
#### Ejecuta el último comando, reemplazando `cadena1` por `cadena2`:
```shell
^{{cadena1}}^{{cadena2}}^
```
#### Realiza una expansión del historial, pero muestra el comando que se ejecutaría en lugar de ejecutarlo realmente:
```shell
{{!-n}}:p
```
{% endraw %}