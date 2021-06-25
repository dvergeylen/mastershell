---
layout: default
title: "mpv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mpv">
  <a href="/it/common/mpv.html">mpv</a> <a href="#mpv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un player audio/video basato su MPlayer.
> Maggiori informazioni: <https://mpv.io>.

#### Riproduci un file video o audio:
```shell
mpv {{file}}
```
#### Salta avanti/indietro di 5 secondi:
```shell
SINISTRA <oppure> DESTRA
```
#### Salta indietro/avanti di 1 minuto:
```shell
GIÙ <oppure> SU
```
#### Riduci o aumenta la velocità di riproduzione del 10%:
```shell
[ <oppure> ]
```
#### Riproduci un file a una velocità specifica (da 0.01 a 100, normalmente 1):
```shell
mpv --speed {{velocità}} {{file}}
```
#### Riproduci un file usando un profilo definito nel file `mpv.conf`:
```shell
mpv --profile {{nome_profilo}} {{file}}
```
{% endraw %}