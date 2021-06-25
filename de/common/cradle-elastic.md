---
layout: default
title: "cradle elastic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-elastic">
  <a href="/de/common/cradle-elastic.html">cradle elastic</a> <a href="#cradle-elastic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte ElasticSearch Instanzen einer Cradle Instanz.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#elastic>.

#### Entleere den ElasticSearch Index:
```shell
cradle elastic flush
```
#### Entleere den ElasticSearch Index für ein bestimmtes Paket:
```shell
cradle elastic flush {{paket}}
```
#### Sende ein ElasticSearch Schema ab:
```shell
cradle elastic map
```
#### Sende ein ElasticSearch Schema für ein bestimmtes Paket ab:
```shell
cradle elastic map {{paket}}
```
#### Befülle die ElasticSearch Indizes für alle Pakete:
```shell
cradle elastic populate
```
#### Befülle die ElasticSearch Indizes für ein bestimmtes Paket:
```shell
cradle elastic populate {{paket}}
```
{% endraw %}