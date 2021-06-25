---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/es/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea alias -- palabras que son remplazadas por una cadena de comando(s).
> Los alias son temporales en la sesión de shell actual, a no ser que estén definidos en el archivo de configuración de la shell, ej. `~/.bashrc`.
> Más información: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Listar todos los alias:
```shell
alias
```
#### Crear un alias genérico:
```shell
alias {{nombre}}="{{comando}}"
```
#### Ver el comando asociado a un alias:
```shell
alias {{nombre}}
```
#### Eliminar un alias (con el comando asociado):
```shell
unalias {{nombre}}
```
#### Convertir `rm` en un comando interactivo:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Crear `la` como un atajo para `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}