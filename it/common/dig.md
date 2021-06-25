---
layout: default
title: "dig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dig">
  <a href="/it/common/dig.html">dig</a> <a href="#dig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilità di lookup DNS.
> Maggiori informazioni: <https://manpages.debian.org/dnsutils/dig.1.html>.

#### Mostra gli IP associati ad un hostname (record A):
```shell
dig +short {{esempio.com}}
```
#### Mostra i mail server associati ad uno specifico dominio (record MX):
```shell
dig +short {{esempio.com}} MX
```
#### Richiedi tutti i tipi di record per un dato dominio:
```shell
dig {{esempio.com}} ANY
```
#### Specifica un server DNS alternativo a cui fare richiesta:
```shell
dig @{{8.8.8.8}} {{esempio.com}}
```
#### Esegui un lookup DNS inverso su di un indirizzo IP (record PTR):
```shell
dig -x {{8.8.8.8}}
```
#### Trova i nameserver autoritativi per la zona e mostra i record SOA:
```shell
dig +nssearch {{esempio.com}}
```
#### Esegui richieste iterative e mostra l'intero percorso per risolvere il dominio:
```shell
dig +trace {{esempio.com}}
```
{% endraw %}