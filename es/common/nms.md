---
layout: default
title: "nms"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nms">
  <a href="/es/common/nms.html">nms</a> <a href="#nms"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de línea de comandos que recrea el famoso efecto de desencriptado de datos de la película Sneakers (1992).
> Más información: <https://github.com/bartobri/no-more-secrets>.

#### Desencripta el texto tras presionar una tecla:
```shell
echo "{{Hola, Mundo!}}" | nms
```
#### Desencripta la salida inmediatamente, sin esperar a que una tecla sea pulsada:
```shell
{{ls -la}} | nms -a
```
#### Desencripta el contenido de un archivo, especificando el color de la salida:
```shell
cat {{ruta/al/archivo}} | nms -a -f {{blue|white|yellow|black|magenta|green|red}}
```
#### Limpia la pantalla antes de desencriptar:
```shell
{{comando}} | nms -a -c
```
{% endraw %}