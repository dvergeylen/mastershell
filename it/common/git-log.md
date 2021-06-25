---
layout: default
title: "git log"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-log">
  <a href="/it/common/git-log.html">git log</a> <a href="#git-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra la cronologia dei commit.
> Maggiori informazioni: <https://git-scm.com/docs/git-log>.

#### Mostra la sequenza dei commit del ramo del repository in uso, a partire dal commit corrente e andando in ordine cronologico inverso:
```shell
git log
```
#### Mostra la cronologia di un dato file o cartella, mostrando anche le modifiche:
```shell
git log -p {{percorso/al/file_o_directory}}
```
#### Offri una panoramica dei file che sono cambiati ad ogni commit:
```shell
git log --stat
```
#### Mostra il grafo dei commit nel ramo corrente, includendo solo la prima riga di ogni messaggio di commit:
```shell
git log --oneline --graph
```
#### Mostra il grafo di tutti i commit, tag e rami dell'intero repository:
```shell
git log --oneline --decorate --all --graph
```
#### Mostra solo i commit il cui messaggio contiene una data stringa (ignorando maiuscole/minuscole):
```shell
git log -i --grep {{stringa_da_cercare}}
```
#### Mostra gli ultimi N commit di un certo autore:
```shell
git log -n {{numero}} --author={{autore}}
```
#### Mostra i commit effettuati tra due date:
```shell
git log --before={{data}} --after={{data}}
```
{% endraw %}