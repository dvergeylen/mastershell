---
layout: default
title: "arping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arping">
  <a href="/it/common/arping.html">arping</a> <a href="#arping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scopri e interroga host in una rete utilizzando il protocollo ARP.
> Utile per scoprire indirizzi MAC.
> Maggiori informazioni: <https://github.com/ThomasHabets/arping>.

#### Invia un ping ad un host inviando pacchetti ARP request:
```shell
arping {{ip_host}}
```
#### Invia un pint ad un host su una specifica interfaccia:
```shell
arping -I {{interfaccia}} {{ip_host}}
```
#### Invia un ping ad un host e termina all prima risposta:
```shell
arping -f {{ip_host}}
```
#### Invia uno specifico numero di ping:
```shell
arping -c {{count}} {{ip_host}}
```
#### Invia pacchetti ARP request in broadcast per aggiornare la cache ARP dei vicini:
```shell
arping -U {{ip_da_inviare_in_broadcast}}
```
#### Rileva indirizzi IP duplicati nella rete inviando richieste ARP con un timeout di 3 secondi:
```shell
arping -D -w {{3}} {{ip_da_controllare}}
```
{% endraw %}