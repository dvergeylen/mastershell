---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/it/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa e concatena file.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/cat>.

#### Stampa i contenuti di un file su standard output:
```shell
cat {{file}}
```
#### Concatena più file in un unico file:
```shell
cat {{file1}} {{file2}} > {{file_finale}}
```
#### Aggiungi il contenuto di diversi file alla fine di un file:
```shell
cat {{file1}} {{file2}} >> {{file_finale}}
```
#### Numera tutte le linee stampate:
```shell
cat -n {{file}}
```
{% endraw %}