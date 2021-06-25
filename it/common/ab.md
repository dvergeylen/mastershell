---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/it/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di benchmarking di Apache. Il più semplice modo per eseguire un test sul carico del server.
> Maggiori informazioni: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Esegui 100 richieste HTTP GET ad un dato URL:
```shell
ab -n {{100}} {{url}}
```
#### Esegui 100 richieste HTTP GET ad un dato URL, processandone fino a 10 contemporaneamente:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Esegui 100 richieste HTTP POST a un dato URL, utilizzando un payload JSON tramite file:
```shell
ab -n {{100}} -T {{application/json}} -p {{percorso/a/file.json}} {{url}}
```
#### Usa HTTP [K]eep Alive, ovvero esegui richieste multiple in una stessa sessione HTTP:
```shell
ab -k {{url}}
```
#### Setta il massimo numero di secondi per il benchmarking:
```shell
ab -t {{secondi}} {{url}}
```
{% endraw %}