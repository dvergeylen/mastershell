---
layout: default
title: "cloc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cloc">
  <a href="/it/common/cloc.html">cloc</a> <a href="#cloc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Conta e calcola le differenze di linee di codice sorgente e commenti.
> Maggiori informazioni: <https://github.com/AlDanial/cloc>.

#### Conta tutte le linee di codice in una directory:
```shell
cloc {{percorso/alla/directory}}
```
#### Conta tutte le linee di codice in una directory, mostrando una barra di avanzamento durante l'operazione:
```shell
cloc --progress=1 {{percorso/alla/directory}}
```
#### Compara i file sorgente in 2 diverse directory e conta le differenze tra di essi:
```shell
cloc --diff {{percorso/a/directory1}} {{percorso/a/directory2}}
```
{% endraw %}