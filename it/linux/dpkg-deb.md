---
layout: default
title: "dpkg-deb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg-deb">
  <a href="/it/linux/dpkg-deb.html">dpkg-deb</a> <a href="#dpkg-deb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Impacchetta, spacchetta e fornisce informazioni su archivi Debian.
> Maggiori informazioni: <https://manpages.debian.org/buster/dpkg/dpkg-deb.1.en.html>.

#### Mostra le informazioni riguardo ad un pacchetto:
```shell
dpkg-deb --info {{percorso/al/file.deb}}
```
#### Mostra il nome e la versione del pacchetto in una singola riga:
```shell
dpkg-deb --show {{percorso/al/file.deb}}
```
#### Elenca i contenuti del pacchetto:
```shell
dpkg-deb --contents {{percorso/al/file.deb}}
```
#### Estrae i contenuti del pacchetto in una cartella:
```shell
dpkg-deb --extract {{percorso/al/file.deb}} {{percorso/alla/cartella}}
```
#### Crea una pacchetto a partire da una cartella specificata:
```shell
dpkg-deb --build {{percorso/alla/cartella}}
```
{% endraw %}