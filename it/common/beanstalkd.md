---
layout: default
title: "beanstalkd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="beanstalkd">
  <a href="/it/common/beanstalkd.html">beanstalkd</a> <a href="#beanstalkd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un semplice e generico gestore di code di lavoro.
> Maggiori informazioni: <https://beanstalkd.github.io/>.

#### Avvia beanstalkd, ascoltando sulla porta 11300:
```shell
beanstalkd
```
#### Avvia beanstalkd ascoltando su porta ed un indirizzo dati:
```shell
beanstalkd -l {{indirizzo_ip}} -p {{numero_porta}}
```
#### Rendi le code di lavoro persistenti salvandole su disco:
```shell
beanstalkd -b {{percorso/a/directory_persistente}}
```
#### Sincronizza con una cartella persistente ogni 500 millisecondi:
```shell
beanstalkd -b {{percorso/a/directory_persistente}} -f {{500}}
```
{% endraw %}