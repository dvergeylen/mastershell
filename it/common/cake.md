---
layout: default
title: "cake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cake">
  <a href="/it/common/cake.html">cake</a> <a href="#cake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento da linea di comando per il framework CakePHP.
> Maggiori informazioni: <https://cakephp.org>.

#### Mostra informazioni sull'attuale app ed i comandi disponibili:
```shell
cake
```
#### Elenca le rotte disponibili:
```shell
cake routes
```
#### Pulisci le cache di configurazione:
```shell
cake cache clear_all
```
#### Costruisci la cache dei metadati:
```shell
cake schema_cache build --connection {{connessione}}
```
#### Pulisci la cache dei metadati:
```shell
cake schema_cache clear
```
#### Pulisci una tabella di cache:
```shell
cake schema_cache clear {{nome_tabella}}
```
#### Avvia un web server di sviluppo (porta predefinita 8765):
```shell
cake server
```
#### Avvia una shell REPL interattiva:
```shell
cake console
```
{% endraw %}