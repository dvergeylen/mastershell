---
layout: default
title: "calibre-server"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calibre-server">
  <a href="/it/common/calibre-server.html">calibre-server</a> <a href="#calibre-server"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un'applicazione server che può essere usata per distribuire e-book in una rete.
> Gli e-book devono prima essere importati nella libreria usando la GUI o calibredb.
> Parte del manager di e-book Calibre.
> Maggiori informazioni: <https://manual.calibre-ebook.com/generated/en/calibre-server.html>.

#### Avvia un server per distribuire e-book. Accesso a http://localhost:8080:
```shell
calibre-server
```
#### Avvia il server su una specifica porta. Accesso a http://localhost:porta:
```shell
calibre-server --port {{porta}}
```
#### Proteggi il server con username e password:
```shell
calibre-server --username {{username}} --password {{password}}
```
{% endraw %}