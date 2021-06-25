---
layout: default
title: "cradle elastic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-elastic">
  <a href="/it/common/cradle-elastic.html">cradle elastic</a> <a href="#cradle-elastic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci le istanze ElasticSearch per un'istanza Cradle.
> Maggiori informazioni: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#elastic>.

#### Svuota l'indice ElasticSearch:
```shell
cradle elastic flush
```
#### Svuota l'indice ElasticSearch per uno specifico pacchetto:
```shell
cradle elastic flush {{nome_pacchetto}}
```
#### Carica lo schema ElasticSearch:
```shell
cradle elastic map
```
#### Carica lo schema ElasticSearch per uno specifico pacchetto:
```shell
cradle elastic map {{nome_pacchetto}}
```
#### Popola gli indici ElasticSearch per tutti i pacchetti:
```shell
cradle elastic populate
```
#### Popola gli indici ElasticSearch per uno specifico pacchetto:
```shell
cradle elastic populate {{nome_pacchetto}}
```
{% endraw %}