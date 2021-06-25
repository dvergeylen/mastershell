---
layout: default
title: "apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt">
  <a href="/it/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Servizio di gestione dei pacchetti per distribuzioni basate su Debian.
> Rimpiazzo raccomandato di apt-get quando usato interattivamente su Ubuntu 16.04 e versioni successive.
> Maggiori informazioni: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Aggiorna la lista dei pacchetti e delle loro versioni disponibili (è consigliato eseguire questo comando prima di altri comandi `apt`):
```shell
sudo apt update
```
#### Cerca per un dato pacchetto:
```shell
apt search {{pacchetto}}
```
#### Mostra le informazioni su un pacchetto:
```shell
apt show {{pacchetto}}
```
#### Installa un pacchetto, o lo aggiorna all'ultima versione disponibile:
```shell
sudo apt install {{pacchetto}}
```
#### Rimuove un pacchetto (usando `purge` rimuove anche i suoi file di configurazione):
```shell
sudo apt remove {{pacchetto}}
```
#### Aggiorna tutti i pacchetti installati alla versione disponibile più recente:
```shell
sudo apt upgrade
```
#### Elenca tutti i pacchetti:
```shell
apt list
```
#### Elenca i pacchetti installati:
```shell
apt list --installed
```
{% endraw %}