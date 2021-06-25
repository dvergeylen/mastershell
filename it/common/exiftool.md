---
layout: default
title: "exiftool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exiftool">
  <a href="/it/common/exiftool.html">exiftool</a> <a href="#exiftool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Leggi e scrivi metadati nei file.
> Maggiori informazioni: <https://owl.phy.queensu.ca/~phil/exiftool>.

#### Rimuovi tutti i metadati EXIF dai file specificati:
```shell
exiftool -All= {{file1 file2 ...}}
```
#### Muovi avanti di 1 ora la data in cui sono state scattate tutte le foto contenute in una directory:
```shell
exiftool "-AllDates+=0:0:0 1:0:0" {{percorso/a/directory}}
```
#### Muovi indietro di 1 giorno e 2 ore la data in cui sono state scattate tutte le immagini JPEG:
```shell
exiftool "-AllDates-=0:0:1 2:0:0" -ext jpg
```
#### Cambia solo il campo `DateTimeOriginal` sottraendo 1.5 ore e non tenere file di backup:
```shell
exiftool -DateTimeOriginal-=1.5 -overwrite_original
```
#### Rinomina ricorsivamente tutti i file JPEG in una directory in base al campo `DateTimeOriginal`:
```shell
exiftool '-filename<DateTimeOriginal' -d %Y-%m-%d_%H-%M-%S%%lc.%%e {{percorso/a/directory}} -r -ext jpg
```
{% endraw %}