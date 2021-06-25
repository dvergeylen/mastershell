---
layout: default
title: "opusenc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="opusenc">
  <a href="/it/common/opusenc.html">opusenc</a> <a href="#opusenc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converte audio WAV o FLAC in Opus.
> Maggiori informazioni: <https://opus-codec.org/docs/opus-tools/opusenc.html>.

#### Converte un file WAV in un file Opus usando le opzioni predefinite:
```shell
opusenc {{percorso/al/file_originale.wav}} {{percorso/al/file_convertito}}.opus
```
#### Converte un audio stereo alla massima qualità possibile:
```shell
opusenc --bitrate {{512}} {{percorso/al/file_originale.wav}} {{percorso/al/file_convertito}}.opus
```
#### Converte un audio con canali surround 5.1 alla massima qualità possibile:
```shell
opusenc --bitrate {{1536}} {{percorso/al/file_originale.flac}} {{percorso/al/file_convertito}}.opus
```
#### Converte l'audio di una voce alla minima qualità possibile:
```shell
opusenc {{percorso/al/file_originale.wav}} --downmix-mono --bitrate {{6}} {{percorso/al/file_convertito}}.opus
```
{% endraw %}