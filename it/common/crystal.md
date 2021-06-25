---
layout: default
title: "crystal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="crystal">
  <a href="/it/common/crystal.html">crystal</a> <a href="#crystal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per gestire codice sorgente Crystal.
> Maggiori informazioni: <https://crystal-lang.org/reference/using_the_compiler>.

#### Esegui un file Crystal:
```shell
crystal {{percorso/al/file.cr}}
```
#### Compila un file e tutte le sue dipendenze in un unico eseguibile:
```shell
crystal build {{percorso/al/file.cr}}
```
#### Avvia un server locale interattivo per testare il linguaggio:
```shell
crystal play
```
#### Crea una directory di progetto per un'applicazione Crystal:
```shell
crystal init app {{nome_applicazione}}
```
#### Mostra tutte le opzioni di aiuto:
```shell
crystal help
```
{% endraw %}