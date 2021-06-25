---
layout: default
title: "bitcoin-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bitcoin-cli">
  <a href="/en/common/bitcoin-cli.html">bitcoin-cli</a> <a href="#bitcoin-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line client to interact with the Bitcoin daemon via RPC calls.
> Uses the configuration defined in `bitcoin.conf`.
> More information: <https://en.bitcoin.it/wiki/Running_Bitcoin#Command-line_arguments>.

#### Send a transaction to a given address:
```shell
bitcoin-cli sendtoaddress "{{address}}" {{amount}}
```
#### Generate one or more blocks:
```shell
bitcoin-cli generate {{num_blocks}}
```
#### Print high-level information about the wallet:
```shell
bitcoin-cli getwalletinfo
```
#### List all outputs from previous transactions available to fund outgoing transactions:
```shell
bitcoin-cli listunspent
```
#### Export the wallet information to a text file:
```shell
bitcoin-cli dumpwallet "{{path/to/file}}"
```
{% endraw %}