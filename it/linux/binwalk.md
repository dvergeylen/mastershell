---
layout: default
title: "binwalk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="binwalk">
  <a href="/it/linux/binwalk.html">binwalk</a> <a href="#binwalk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per l'analisi di file binari.
> Maggiori informazioni: <https://github.com/ReFirmLabs/binwalk>.

#### Scansiona un file binario:
```shell
binwalk {{percorso/a/file}}
```
#### Estrae file da un binario, specificando la cartella di output:
```shell
binwalk --extract --directory {{cartella_di_output}} {{percorso/a/file}}
```
#### Estrae file in maniera ricorsiva a partire da un binario, limitando la profondità di ricorsione a 2 livelli:
```shell
binwalk --extract --matryoshka --depth {{2}} {{percorso/a/file}}
```
#### Estrae file da un binario utilizzando una particolare firma (ad esempio il MIME Type):
```shell
binwalk --dd '{{png image:png}}' {{percorso/a/file}}
```
#### Analizza l'entropia di un binario e salva il grafico con lo stesso filename del binario, con l'estensione `.png` in fondo:
```shell
binwalk --entropy --save {{percorso/a/file}}
```
#### Combina analisi di entropia, firme e opcode in un unico comando:
```shell
binwalk --entropy --signature --opcodes {{percorso/a/file}}
```
{% endraw %}