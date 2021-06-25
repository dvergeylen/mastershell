---
layout: default
title: "spotify"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="spotify">
  <a href="/es/osx/spotify.html">spotify</a> <a href="#spotify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Una línea de comando para Spotify.
> Más información: <https://github.com/hnarayanan/shpotify>.

#### Encuentra una canción por su nombre y la reproduce:
```shell
spotify play {{song_name}}
```
#### Encuentra una lista de reproducción por su nombre y la reproduce:
```shell
spotify play list {{playlist_name}}
```
#### Pausa (o reanuda) la reproducción:
```shell
spotify pause
```
#### Pasa a la siguiente canción de una lista de reproducción:
```shell
spotify next
```
#### Cambia el volumen:
```shell
spotify vol {{up|down|value}}
```
#### Muestra el estado de reproducción y los detalles de la canción:
```shell
spotify status
```
{% endraw %}