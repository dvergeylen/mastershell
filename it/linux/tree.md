---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/it/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra i contenuti della cartella corrente come un albero.
> Maggiori informazioni: <http://mama.indstate.edu/users/ice/tree/>.

#### Stampa file e cartella fino al 'num'-esimo livello di profondità (dove 1 significa la cartella corrente):
```shell
tree -L {{num}}
```
#### Stampa solamente le cartelle:
```shell
tree -d
```
#### Stampa anche i file nascosti con la colorazione attiva:
```shell
tree -a -C
```
#### Stampa l'albero senza linee di indentazione, mostrando invece il percorso completo (usa `-N` per non convertire caratteri non stampabili in sequenze di escape):
```shell
tree -i -f
```
#### Stampa la dimensione di ogni file e la dimensione totale di ogni cartella, in formato leggibile dall'utente:
```shell
tree -s -h --du
```
#### Stampa i file all'interno dell'albero gerarchico, utilizzando espressioni di metacaratteri (glob pattern) per escludere le cartelle che non contengono file corrispondenti alla ricerca:
```shell
tree -P '{{*.txt}}' --prune
```
#### Stampa le cartelle all'interno dell'albero gerarchico, utilizzando espressioni di metacaratteri (glob pattern) per escludere le cartelle che non sono progenitori di quelle desiderate:
```shell
tree -P {{nomi_di_cartelle}} --matchdirs --prune
```
#### Stampa l'albero ignorando le cartelle date:
```shell
tree -I '{{nome_cartella1|nome_cartella2}}'
```
{% endraw %}