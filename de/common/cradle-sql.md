---
layout: default
title: "cradle sql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-sql">
  <a href="/de/common/cradle-sql.html">cradle sql</a> <a href="#cradle-sql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Cradle SQL Datenbanken.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#sql>.

#### Generiere ein neues Datenbank-Schema:
```shell
cradle sql build
```
#### Generiere ein neues Datenbank-Schema für ein bestimmtes Paket:
```shell
cradle sql build {{paket}}
```
#### Entleere die gesamte Datenbank:
```shell
cradle sql flush
```
#### Entleere die Datenbank für ein bestimmtes Paket:
```shell
cradle sql flush {{paket}}
```
#### Befülle die Tabellen für alle Pakete:
```shell
cradle sql populate
```
#### Befülle die Tabellen für ein bestimmtes Paket:
```shell
cradle sql populate {{paket}}
```
{% endraw %}