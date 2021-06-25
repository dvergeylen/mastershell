---
layout: default
title: "cordova"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cordova">
  <a href="/it/common/cordova.html">cordova</a> <a href="#cordova"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Applicazioni mobile con HTML, CSS e JavaScript.
> Maggiori informazioni: <https://cordova.apache.org/docs/en/latest/guide/cli/>.

#### Crea un progetto Cordova:
```shell
cordova create {{percorso}} {{nome_pacchetto}} {{nome_progetto}}
```
#### Mostra lo stato della workspace corrente:
```shell
cordova info
```
#### Aggiungi una piattaforma Cordova:
```shell
cordova platform add {{piattaforma}}
```
#### Rimuovi una piattaforma Cordova:
```shell
cordova platform remove {{piattaforma}}
```
#### Aggiungi un plugin Cordova:
```shell
cordova plugin add {{id_plugin}}
```
#### Rimuovi un plugin Cordova:
```shell
cordova plugin remove {{id_plugin}}
```
{% endraw %}