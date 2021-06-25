---
layout: default
title: "vim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vim">
  <a href="/it/common/vim.html">vim</a> <a href="#vim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vi IMproved, un editor di testo per programmatori che fornisce diverse modalità per modificare testo.
> Premi `i` per entrare in insert mode e `<Esc>` per tornare in normal mode dove non puoi inserire testo normalmente.
> Maggiori informazioni: <https://www.vim.org>.

#### Apri un file in vim:
```shell
vim {{file}}
```
#### Vai in insert mode (per inserire testo):
```shell
<Esc>i
```
#### Copia ("yank") o taglia ("delete") la linea corrente (per incollarla poi con `P`):
```shell
<Esc>{{yy|dd}}
```
#### Annulla l'ultima operazione:
```shell
<Esc>u
```
#### Cerca un pattern nel file (usa `n`/`N` per spostarti al risultato successivo/precedente):
```shell
<Esc>/{{espressione_regolare}}<Invio>
```
#### Effettua una sostituzione tramite espressione regolare nell'intero file:
```shell
<Esc>:%s/{{espressione_regolare}}/{{sostituzione}}/g<Invio>
```
#### Salva modifiche al file ed esci:
```shell
<Esc>:wq<Invio>
```
#### Esci senza salvare:
```shell
<Esc>:q!<Invio>
```
{% endraw %}