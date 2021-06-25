---
layout: default
title: "couchdb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="couchdb">
  <a href="/it/common/couchdb.html">couchdb</a> <a href="#couchdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfaccia da linea di comando per il server di database Apache CouchDB.
> Maggiori informazioni: <https://couchdb.apache.org>.

#### Avvia couchdb:
```shell
couchdb
```
#### Avvia una shell couchdb interattiva:
```shell
couchdb -i
```
#### Avvia couchdb come processo in background:
```shell
couchdb -b
```
#### Termina il processo in background (nota: si riavvierà da solo se necessario):
```shell
couchdb -k
```
#### Disattiva il processo in background:
```shell
couchdb -d
```
{% endraw %}