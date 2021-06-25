---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/it/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa e concatena file.
> Un clone di `cat` con syntax highlighting e integrazione Git.

#### Stampa i contenuti di un file su standard output:
```shell
bat {{file}}
```
#### Concatena diversi file in un unico file:
```shell
bat {{file1}} {{file2}} > {{file_finale}}
```
#### Aggiungi il contenuto di diversi file alla fine di un file:
```shell
bat {{file1}} {{file2}} >> {{file_finale}}
```
#### Numera tutte le linee stampate:
```shell
bat -n {{file}}
```
#### Evidenzia la sintassi di un file JSON:
```shell
bat --language json {{file.json}}
```
#### Mostra tutti i linguaggi supportati:
```shell
bat --list-languages
```
{% endraw %}