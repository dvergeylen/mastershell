---
layout: default
title: "cradle sql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-sql">
  <a href="/it/common/cradle-sql.html">cradle sql</a> <a href="#cradle-sql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci database SQL di Cradle.
> Maggiori informazioni: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#sql>.

#### Ricostruisci lo schema del database:
```shell
cradle sql build
```
#### Ricostruisci lo schema del database per uno specifico pacchetto:
```shell
cradle sql build {{nome_pacchetto}}
```
#### Svuota l'intero database:
```shell
cradle sql flush
```
#### Svuota le tabelle del database per uno specifico pacchetto:
```shell
cradle sql flush {{nome_pacchetto}}
```
#### Popola le tabelle per tutti i pacchetti:
```shell
cradle sql populate
```
#### Popola le tabelle per uno specifico pacchetto:
```shell
cradle sql populate {{nome_pacchetto}}
```
{% endraw %}