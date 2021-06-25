---
layout: default
title: "bitcoin-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bitcoin-cli">
  <a href="/it/common/bitcoin-cli.html">bitcoin-cli</a> <a href="#bitcoin-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Client da linea di comando per interagire con il demone Bitcoin tramite chiamate RPC.
> Utilizza la configurazione definita in `bitcoin.conf`.
> Maggiori informazioni: <https://en.bitcoin.it/wiki/Running_Bitcoin#Command-line_arguments>.

#### Invia una transazione ad un dato indirizzo:
```shell
bitcoin-cli sendtoaddress "{{indirizzo}}" {{importo}}
```
#### Genera uno o più blocchi:
```shell
bitcoin-cli generate {{numero_blocchi}}
```
#### Mostra informazioni di alto livello sul portafogli:
```shell
bitcoin-cli getwalletinfo
```
#### Elenca tutti gli output di transazioni precedenti disponibili per finanziare una nuove transazioni:
```shell
bitcoin-cli listunspent
```
#### Esporta le informazioni sul portafogli in un file di testo:
```shell
bitcoin-cli dumpwallet "{{percorso/al/file}}"
```
{% endraw %}