---
layout: default
title: "apt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-get">
  <a href="/it/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio di gestione dei pacchetti per Debian e Ubuntu.
> Cerca i pacchetti usando `apt-cache`.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Aggiorna la lista dei pacchetti e delle loro versioni disponibili (è consigliato eseguire questo comando prima di altri comandi `apt-get`):
```shell
apt-get update
```
#### Installa un pacchetto, o lo aggiorna all'ultima versione disponibile:
```shell
apt-get install {{pacchetto}}
```
#### Rimuove un pacchetto:
```shell
apt-get remove {{pacchetto}}
```
#### Rimuove un pacchetto ed i suoi file di configurazione:
```shell
apt-get purge {{pacchetto}}
```
#### Aggiorna tutti i pacchetti installati alla versione disponibile più recente:
```shell
apt-get upgrade
```
#### Pulisce gli archivi locali - rimuovendo i file (.deb) da scaricamenti interrotti che non possono più essere scaricati:
```shell
apt-get autoclean
```
#### Rimuove tutti i pacchetti che non sono più necessari:
```shell
apt-get autoremove
```
#### Aggiorna tutti i pacchetti installati (come `upgrade`), rimuovendo i pacchetti obsoleti ed installando ulteriori pacchetti per soddisfare le nuove dipendenze:
```shell
apt-get dist-upgrade
```
{% endraw %}