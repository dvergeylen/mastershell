---
layout: default
title: "bitcoin-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bitcoin-cli">
  <a href="/pl/common/bitcoin-cli.html">bitcoin-cli</a> <a href="#bitcoin-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Klient konsolowy do interakcji z demonem Bitcoina poprzez zapytania RPC.
> Używa konfiguracji zdefiniowanej w `bitcoin.conf`.
> Więcej informacji: <https://en.bitcoin.it/wiki/Running_Bitcoin#Command-line_arguments>.

#### Wyślij transakcję na dany adres:
```shell
bitcoin-cli sendtoaddress "{{adres}}" {{ilość}}
```
#### Wygeneruj jeden lub więcej bloków:
```shell
bitcoin-cli generate {{ilość_bloków}}
```
#### Wyświetl informacje o portfelu:
```shell
bitcoin-cli getwalletinfo
```
#### Wyświetl wszystkie poprzednie transakcje dostępne do opłacenia transakcji wychodzących:
```shell
bitcoin-cli listunspent
```
#### Wyeksportuj dane portfela do pliku tekstowego:
```shell
bitcoin-cli dumpwallet "{{ścieżka/do/pliku}}"
```
{% endraw %}