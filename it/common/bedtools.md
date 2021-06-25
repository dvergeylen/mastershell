---
layout: default
title: "bedtools"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bedtools">
  <a href="/it/common/bedtools.html">bedtools</a> <a href="#bedtools"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un coltellino svizzero di strumenti per analisi genomica.
> Usato per intersecare, raggruppare, convertire e contare dati in formato BAM, BED, GFF/GTF, VCF.
> Maggiori informazioni: <https://bedtools.readthedocs.io/en/latest/>.

#### Interseca i fili genetici delle sequenze contenute in due file diversi e salva il risultato:
```shell
bedtools intersect -a {{percorso/al/file_1}} -b {{percorso/al/file_2}} -s > {{percorso/al/file_output}}
```
#### Interseca due file unendo il risultato a sinistra, ovvero riporta ogni feature da {{file_1}} e NULL dove non c'è sovrapposizione con {{file_2}}:
```shell
bedtools intersect -a {{percorso/al/file_1}} -b {{percorso/al/file_2}} -lof > {{percorso/al/file_output}}
```
#### Usa un algoritmo più efficiente per intersecare due file precedentemente ordinati:
```shell
bedtools intersect -a {{percorso/al/file_1}} -b {{percorso/al/file_2}} -sorted > {{percorso/al/file_output}}
```
#### Raggruppa file in base alle prime tre e la quinta colonna e raggruppa la sesta colonna sommandola:
```shell
bedtools groupby -i {{percorso/al/file}} -c 1-3,5 -g 6 -o sum
```
#### Converti da formato BAM a BED:
```shell
bedtools bamtobed -i {{percorso/al/file}}.bam > {{percorso/al/file}}.bed
```
#### Trova per tutte le proprietà in {{file_1}} la più vicina in {{file_2}} e scrivi la loro distanza in una ulteriore colonna (i file in input devono essere ordinati):
```shell
bedtools closest -a {{percorso/al/file_1}}.bed -b {{percorso/al/file_2}}.bed -d
```
{% endraw %}