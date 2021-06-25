---
layout: default
title: "cradle package"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-package">
  <a href="/it/common/cradle-package.html">cradle package</a> <a href="#cradle-package"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci pacchetti per un'istanza Cradle.
> Maggiori informazioni: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#package>.

#### Mostra una lista dei pacchetti disponibili:
```shell
cradle package list
```
#### Cerca un pacchetto:
```shell
cradle package search {{pacchetto}}
```
#### Installa un pacchetto da Packagist:
```shell
cradle package install {{pacchetto}}
```
#### Installa una specifica versione di un pacchetto:
```shell
cradle package install {{pacchetto}} {{versione}}
```
#### Aggiorna un pacchetto:
```shell
cradle package update {{pacchetto}}
```
#### Aggiorna un pacchetto ad una specifica versione:
```shell
cradle package update {{pacchetto}} {{versione}}
```
#### Rimuovi uno specifico pacchetto:
```shell
cradle package remove {{pacchetto}}
```
{% endraw %}