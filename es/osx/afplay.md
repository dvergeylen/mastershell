---
layout: default
title: "afplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="afplay">
  <a href="/es/osx/afplay.html">afplay</a> <a href="#afplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reproductor de audio de línea de comandos.

#### Reproduce un archivo de audio (espera hasta que finalice la reproducción):
```shell
afplay {{ruta/al/archivo}}
```
#### Reproduce un archivo de audio a una velocidad 2x (velocidad de reproducción):
```shell
afplay --rate {{2}} {{ruta/al/archivo}}
```
#### Reproduce un archivo de audio a la mitad de velocidad:
```shell
afplay --rate {{0.5}} {{ruta/al/archivo}}
```
#### Reproduce los primeros N segundos de un archivo de audio:
```shell
afplay --time {{segundos}} {{ruta/al/archivo}}
```
{% endraw %}