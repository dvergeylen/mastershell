---
layout: default
title: "apt-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-cache">
  <a href="/it/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumenti di Debian e Ubuntu per richiedere informazioni sui pacchetti.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Cerca un pacchetto nelle sorgenti attuali:
```shell
apt-cache search {{query}}
```
#### Mostra informazioni su un pacchetto:
```shell
apt-cache show {{pacchetto}}
```
#### Mostra se un pacchetto è installato ed aggiornato:
```shell
apt-cache policy {{pacchetto}}
```
#### Mostra le dipendenze di un pacchetto:
```shell
apt-cache depends {{pacchetto}}
```
#### Mostra i pacchetti che dipendono da un particolare pacchetto:
```shell
apt-cache rdepends {{pacchetto}}
```
{% endraw %}