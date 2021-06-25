---
layout: default
title: "id3tag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="id3tag">
  <a href="/it/common/id3tag.html">id3tag</a> <a href="#id3tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per leggere, scrivere, e manipolare i tag (etichette) ID3v1 e ID3v2 di file MP3.

#### Imposta l'etichetta dell'artista e del titolo in un file MP3:
```shell
id3tag --artist={{artista}} --title={{titolo}} {{percorso/al/file.mp3}}
```
#### Imposta il titolo dell'album di tutti i file MP3 nella cartella corrente:
```shell
id3tag --album={{album}} {{*.mp3}}
```
#### Fornisce altro aiuto:
```shell
id3tag --help
```
{% endraw %}