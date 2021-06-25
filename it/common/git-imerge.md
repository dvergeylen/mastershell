---
layout: default
title: "git-imerge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-imerge">
  <a href="/it/common/git-imerge.html">git-imerge</a> <a href="#git-imerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui un'unione (merge) o rebase tra due rami Git in modo incrementale.
> Eventuali conflitti tra i due rami sono tracciati in coppie di commit distinti, per semplificarne la risoluzione.
> Maggiori informazioni: <https://github.com/mhagger/git-imerge>.

#### Avvia un rebase usando imerge (dopo aver fatto checkout sul ramo da spostare):
```shell
git imerge rebase {{ramo_su_cui_eseguire_il_rebase}}
```
#### Avvia un'unione usando imerge (dopo aver fatto checkout sul ramo di destinazione):
```shell
git imerge merge {{ramo_da_unire}}
```
#### Mostra con un diagramma ASCII lo stato di esecuzione dell'unione o rebase:
```shell
git imerge diagram
```
#### Continua con l'operazione di imerge dopo aver risolto i conflitti (dopo aver aggiunto i file in conflitto con `git add`):
```shell
git imerge continue --no-edit
```
#### Concludi l'operazione di imerge dopo aver risolto tutti i conflitti:
```shell
git imerge finish
```
#### Interrompi l'operazione di imerge e ritorna al ramo precedente:
```shell
git-imerge remove && git checkout {{ramo_precedente}}
```
{% endraw %}