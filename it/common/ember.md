---
layout: default
title: "ember"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ember">
  <a href="/it/common/ember.html">ember</a> <a href="#ember"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilità da lina di comando per Ember.js.
> Utilizzato per creare e mantenere applicazioni Ember.js.
> Maggiori informazioni: <https://cli.emberjs.com>.

#### Crea una nuova applicazione Ember:
```shell
ember new {{nome_app}}
```
#### Crea un nuovo addon Ember:
```shell
ember addon {{nome_addon}}
```
#### Builda un progetto:
```shell
ember build
```
#### Builda un progetto in modalità produzione:
```shell
ember build -prod
```
#### Avvia un server di sviluppo:
```shell
ember serve
```
#### Esegui una suite di test:
```shell
ember test
```
#### Esegui un blueprint per generare una route o un componente:
```shell
ember generate {{tipo}} {{nome}}
```
#### Installa un addon ember-cli:
```shell
ember install {{nome_addon}}
```
{% endraw %}