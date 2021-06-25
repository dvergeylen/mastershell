---
layout: default
title: "nvim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nvim">
  <a href="/it/common/nvim.html">nvim</a> <a href="#nvim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Neovim, un editor di testo basato su Vim che offre molti diversi modi di manipolare e navigare il testo.
> Premere `i` per entrare in modalità inserimento (insert mode), `<Esc>` per uscire e tornare alla modalità normale (normal mode).
> Maggiori informazioni: <https://neovim.io>.

#### Aprire un file:
```shell
nvim {{file}}
```
#### Entrare nella modalità per scrivere testo (insert mode):
```shell
<Esc>i
```
#### Copiare ("yank") o cancellare ("delete") la linea corrente (può poi essere copiara con `p` o `P`):
```shell
<Esc>{{yy|dd}}
```
#### Annullare l'ultima operazione fatta:
```shell
<Esc>u
```
#### Cercare uno specifico pattern nel file (premere `n`/`N` per navigare tra le occorrenze successive/precedenti):
```shell
<Esc>/{{patter_da_cercare}}<Enter>
```
#### Eseguire una sostituzione tramite espressione regolare nell'intero file:
```shell
<Esc>:%s/{{espressione_regolare}}/{{sostituzione}}//g<Enter>
```
#### Salvare (scrivere) il file per poi uscire:
```shell
<Esc>:wq<Enter>
```
#### Uscire senza salvare:
```shell
<Esc>:q!<Enter>
```
{% endraw %}