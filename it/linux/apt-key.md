---
layout: default
title: "apt-key"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-key">
  <a href="/it/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio di gestione delle chiavi per il gestore di pacchetti APT su Debian ed Ubuntu.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### Elenca le chiavi fidate:
```shell
apt-key list
```
#### Aggiunge una chiave al portachiavi delle chiavi fidate:
```shell
apt-key add {{file_chiave_pubblica.asc}}
```
#### Elimina una chiave dal portachiavi delle chiavi fidate:
```shell
apt-key del {{id_chiave}}
```
#### Aggiunge una chiave remota al portachiavi delle chiavi fidate:
```shell
wget -qO - {{https://indirizzo.tld/filename.key}} | apt-key add -
```
#### Aggiunge una chiave da un server di chiavi con il solo id della chiave:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{ID_DELLA_CHIAVE}}
```
{% endraw %}