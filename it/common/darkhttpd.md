---
layout: default
title: "darkhttpd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="darkhttpd">
  <a href="/it/common/darkhttpd.html">darkhttpd</a> <a href="#darkhttpd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Web server Darkhttpd.
> Maggiori informazioni: <https://unix4lyfe.org/darkhttpd>.

#### Avvia il server utilizzando la directory specificata come document root:
```shell
darkhttpd {{percorso/a/docroot}}
```
#### Avvia il server su una specifica porta (8080 di default per utenti non root):
```shell
darkhttpd {{percorso/a/docroot}} --port {{porta}}
```
#### Ascolta solo su uno specifico indirizzo IP (di default, il server ascolta su tutte le interfacce):
```shell
darkhttpd {{percorso/a/docroot}} --addr {{indirizzo_ip}}
```
{% endraw %}