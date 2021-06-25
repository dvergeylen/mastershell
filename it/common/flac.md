---
layout: default
title: "flac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flac">
  <a href="/it/common/flac.html">flac</a> <a href="#flac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codifica, decodifica e controlla file flac.
> Maggiori informazioni: <https://xiph.org/flac>.

#### Converte un file wav in un file flac (questo creerà un file flac nella medesima posizione del file wav):
```shell
flac {{percorso/al/file.wav}}
```
#### Codifica un file wav in flac, specificando il nome del risultato:
```shell
flac -o {{percorso/al/file_compresso.flac}} {{percorso/al/file_originale.wav}}
```
#### Decodifica un file wav in flac, specificando il nome del risultato:
```shell
flac -d -o {{percorso/al/file_decompresso.wav}} {{percorso/al/file_originale.flac}}
```
#### Controlla che un file flac sia codificato correttamente:
```shell
flac -t {{percorso/al/file.flac}}
```
{% endraw %}