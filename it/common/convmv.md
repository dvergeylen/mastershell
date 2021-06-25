---
layout: default
title: "convmv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convmv">
  <a href="/it/common/convmv.html">convmv</a> <a href="#convmv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Coversione dei nomi dei file (NON del contenuto) da un encoding ad un altro.
> Maggiori informazioni: <https://www.j3e.de/linux/convmv/man/>.

#### Controlla la conversione di encoding (non rinomina realmente il file):
```shell
convmv -f {{encoding_originale}} -t {{encoding_finale}} {{file_input}}
```
#### Converti l'encoding del nome di un file e rinominalo utilizzando il nuovo encoding:
```shell
convmv -f {{encoding_originale}} -t {{encoding_finale}} --notest {{file_input}}
```
{% endraw %}