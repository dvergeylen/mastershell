---
layout: default
title: "git rebase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rebase">
  <a href="/it/common/git-rebase.html">git rebase</a> <a href="#git-rebase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Applica i commit di un ramo su un ramo differente.
> Tipicamente usato per riallineare (rebase) due rami, creando copie dei commit nella nuova posizione.
> Maggiori informazioni: <https://git-scm.com/docs/git-rebase>.

#### Riallinea il ramo corrente con il ramo specificato:
```shell
git rebase {{ramo_della_nuova_base}}
```
#### Avvia un rebase interattivo, che consente di riordinare, omettere, unire o modificare i commit:
```shell
git rebase -i {{nome_ramo_o_commit_hash}}
```
#### Prosegui con un rebase che era stato sospeso da un errore di unione, dopo aver risolto i conflitti:
```shell
git rebase --continue
```
#### Prosegui con un rebase che era stato sospeso da conflitti di unione, ignorando i commit in conflitto:
```shell
git rebase --skip
```
#### Interrompi un rebase in corso (ad esempio perché interrotto da un conflitto di unione):
```shell
git rebase --abort
```
#### Sposta parti del ramo corrente su una base differente, specificando la vecchia base di partenza:
```shell
git rebase --onto {{nuova_base}} {{vecchia_base}}
```
#### Applica gli ultimi 5 commit locali, consentendo di riordinarli, ometterli, unirli o modificarli:
```shell
git rebase -i {{HEAD~5}}
```
#### Risolvi automaticamente i conflitti a favore del ramo di versione corrente (la parola chiave `theirs` ha qui un significato opposto):
```shell
git rebase -X theirs {{nome_ramo}}
```
{% endraw %}