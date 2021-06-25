---
layout: default
title: "conky"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="conky">
  <a href="/es/linux/conky.html">conky</a> <a href="#conky"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor de sistema ligero para X.
> Más información: <https://github.com/brndnmtthws/conky>.

#### Ejecuta con la configuración por defecto:
```shell
conky
```
#### Crea una nueva configuración por defecto:
```shell
conky -C > ~/.conkyrc
```
#### Ejecuta conky con un archivo de configuración concreto:
```shell
conky -c {{ruta/a/la/configuración}}
```
#### Ejecuta en segundo plano (*daemon*):
```shell
conky -d
```
#### Alinea conky en el escritorio:
```shell
conky -a {{{arriba,abajo,en_medio}_{izquierda,derecha,en_medio}}}
```
#### Pausa de 5 segundos al inciar antes de ejecutarlo:
```shell
conky -p {{5}}
```
{% endraw %}