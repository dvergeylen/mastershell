---
layout: default
title: "git checkout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-checkout">
  <a href="/it/common/git-checkout.html">git checkout</a> <a href="#git-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia rami o ripristina i file dell'albero di lavoro.
> Maggiori informazioni: <https://git-scm.com/docs/git-checkout>.

#### Crea e passa ad un nuovo ramo:
```shell
git checkout -b {{nome_ramo}}
```
#### Crea e passa ad un nuovo ramo a partire dal riferimento specificato (ramo-locale, remote/ramo-remoto, tag sono alcuni esempi di riferimenti validi):
```shell
git checkout -b {{nome_ramo}} {{riferimento}}
```
#### Passa ad un ramo locale esistente:
```shell
git checkout {{nome_ramo}}
```
#### Passa ad un ramo remoto esistente:
```shell
git checkout --track {{nome_repository_remoto}}/{{nome_ramo}}
```
#### Annulla tutte le modifiche nella cartella corrente che non sono state aggiunte all'area di stage (vedi `git reset` per più comandi simili):
```shell
git checkout .
```
#### Annulla tutte le modifiche di un dato file non aggiunte all'area di stage:
```shell
git checkout {{nome_file}}
```
#### Sostituisci un file con il contenuto del suo corrispondente localizzato su un altro ramo:
```shell
git checkout {{nome_ramo}} -- {{nome_file}}
```
{% endraw %}