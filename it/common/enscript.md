---
layout: default
title: "enscript"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="enscript">
  <a href="/it/common/enscript.html">enscript</a> <a href="#enscript"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converti file di testo in PostScript, HTML, RTF, ANSI ed overstrike.
> Maggiori informazioni: <https://www.gnu.org/software/enscript>.

#### Genera un file PostScript da un file di testo:
```shell
enscript {{percorso/a/file_input}} --output={{percorso/a/file_output}}
```
#### Genera un file in un linguaggio differente da PostScript:
```shell
enscript {{percorso/a/file_input}} --language={{linguaggio}} --output={{percorso/a/file_output}}
```
#### Genera un file PostScript con layout orizzontale, dividendo la pagina in colonne (massimo 9):
```shell
enscript {{percorso/a/file_input}} --columns={{numero_colonne}} --landscape --output={{percorso/a/file_output}}
```
#### Mostra linguaggi e formati file disponibili per evidenziare la sintassi:
```shell
enscript --help-highlight
```
#### Genera un file PostScript con evidenziazione della sintassi e colori per uno specifico linguaggio:
```shell
enscript {{percorso/a/file_input}} --color=1 --highlight={{linguaggio}} --output={{percorso/a/file_output}}
```
{% endraw %}