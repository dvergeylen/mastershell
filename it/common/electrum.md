---
layout: default
title: "electrum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="electrum">
  <a href="/it/common/electrum.html">electrum</a> <a href="#electrum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ergonomico wallet (portafogli) Bitcoin e gestore di chiavi private.
> Maggiori informazioni: <https://electrum.org>.

#### Crea un nuovo wallet:
```shell
electrum -w {{nuovo_wallet.dat}} create
```
#### Ripristina un wallet esistente da un seed offline:
```shell
electrum -w {{wallet_ripristinato.dat}} restore -o
```
#### Crea una transazione firmata offline:
```shell
electrum mktx {{destinatario}} {{ammontare}} -f 0.0000001 -F {{mittente}} -o
```
#### Mostra tutti gli indirizzi del wallet per la ricezione:
```shell
electrum listaddresses -a
```
#### Firma un messaggio:
```shell
electrum signmessage {{indirizzo}} {{messaggio}}
```
#### Verifica un messaggio:
```shell
electrum verifymessage {{indirizzo}} {{firma}} {{messaggio}}
```
#### Connettiti solo ad una specifica istanza electrum-server:
```shell
electrum -p socks5:{{127.0.0.1}}:9050 -s {{56ckl5obj37gypcu.onion}}:50001:t -1
```
{% endraw %}