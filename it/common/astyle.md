---
layout: default
title: "astyle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="astyle">
  <a href="/it/common/astyle.html">astyle</a> <a href="#astyle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Indentatore, formattatore e beautifier di codice sorgente per i linguaggi C, C++, C# e Java.
> Quando eseguito, una copia del file originale è creata con l'estensione ".orig" aggiunta come suffisso.
> Maggiori informazioni: <http://astyle.sourceforge.net/>.

#### Applica lo stile di default di 4 spazi per livello di indentazione e nessun cambiamento alla formattazione:
```shell
astyle {{file_sorgente}}
```
#### Applica lo stile java con parentesi graffe aperte sulla stessa riga (attached braces):
```shell
astyle --style=java {{percorso/al/file}}
```
#### Applica lo stile allman per parantesi graffe su linee separate (broken braces):
```shell
astyle --style=allman {{percorso/al/file}}
```
#### Applica un'indentazione personalizzata utilizzando spazi. Scegli tra 2 e 20 spazi:
```shell
astyle --indent=spaces={{numero_spazi}} {{percorso/al/file}}
```
#### Applica un'indentazione personalizzata utilizzando tab. Scegli tra 2 e 20 tab:
```shell
astyle --indent=tab={{numero_tab}} {{percorso/al/file}}
```
{% endraw %}