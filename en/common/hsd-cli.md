---
layout: default
title: "hsd-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hsd-cli">
  <a href="/en/common/hsd-cli.html">hsd-cli</a> <a href="#hsd-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The command-line REST tool for the Handshake blockchain.
> More information: <https://handshake.org>.

#### Retrieve information about the current server:
```shell
hsd-cli info
```
#### Broadcast a local transaction:
```shell
hsd-cli broadcast {{transaction_hex}}
```
#### Retrieve a mempool snapshot:
```shell
hsd-cli mempool
```
#### View a transaction by address or hash:
```shell
hsd-cli tx {{address_or_hash}}
```
#### View a coin by its hash index or address:
```shell
hsd-cli coin {{hash_index_or_address}}
```
#### View a block by height or hash:
```shell
hsd-cli block {{height_or_hash}}
```
#### Reset the chain to the specified block:
```shell
hsd-cli reset {{height_or_hash}}
```
#### Execute an RPC command:
```shell
hsd-cli rpc {{command}} {{args}}
```
{% endraw %}