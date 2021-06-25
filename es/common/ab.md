---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/es/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta comparativa del servidor Apache HTTP.
> Más información: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Ejecuta 100 solicitudes HTTP GET a una URL dada:
```shell
ab -n {{100}} {{url}}
```
#### Ejecuta 100 solicitudes HTTP GET, en lotes simultáneos de a 10, a una URL:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Ejecuta 100 solicitudes HTTP POST a una URL, utilizando la carga JSON de un archivo:
```shell
ab -n {{100}} -T {{application/json}} -p {{ruta/al/archivo.json}} {{url}}
```
#### Utiliza HTTP [K]eep Alive, es decir, realiza múltiples solitudes dentro de una sesión HTTP:
```shell
ab -k {{url}}
```
#### Establece el máximo número de segundos utilizados para la comparación.
```shell
ab -t {{60}} {{url}}
```
{% endraw %}