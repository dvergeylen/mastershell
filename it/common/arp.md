---
layout: default
title: "arp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp">
  <a href="/it/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra e gestisci la cache ARP di sistema.
> Maggiori informazioni: <https://manned.org/arp>.

#### Mostra la tabella ARP corrente:
```shell
arp -a
```
#### Elimina l'intera cache:
```shell
sudo arp -a -d
```
#### Elimina una specifica voce:
```shell
arp -d {{indirizzo}}
```
#### Crea una nuova voce:
```shell
arp -s {{indirizzo}} {{indirizzo_mac}}
```
{% endraw %}