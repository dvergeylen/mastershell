---
layout: default
title: "behat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="behat">
  <a href="/it/common/behat.html">behat</a> <a href="#behat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un framework PHP per lo sviluppo quidato dal comportamento.
> Maggiori informazioni: <https://behat.org>.

#### Inizializza un nuovo progetto Behat:
```shell
behat --init
```
#### Esegui tutti i test:
```shell
behat
```
#### Esegui tutti i test di una specifica suite:
```shell
behat --suite={{nome_suite}}
```
#### Esegui i test con uno specifico formato di output:
```shell
behat --format {{pretty|progress}}
```
#### Esegui i testi e scrivi i risultati in un file:
```shell
behat --out {{percorso/a/file}}
```
#### Mostra una lista delle definizioni nelle suite di test:
```shell
behat --definitions
```
{% endraw %}