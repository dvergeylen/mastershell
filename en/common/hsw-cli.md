---
layout: default
title: "hsw-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hsw-cli">
  <a href="/en/common/hsw-cli.html">hsw-cli</a> <a href="#hsw-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The command-line REST tool for the Handshake wallet.
> More information: <https://npmjs.com/package/hs-client>.

#### Unlock the current wallet (timeout in seconds):
```shell
hsw-cli unlock {{passphrase}} {{timeout}}
```
#### Lock the current wallet:
```shell
hsw-cli lock
```
#### View the current wallet's details:
```shell
hsw-cli get
```
#### View the current wallet's balance:
```shell
hsw-cli balance
```
#### View the current wallet's transaction history:
```shell
hsw-cli history
```
#### Send a transaction with the specified coin amount to an address:
```shell
hsw-cli send {{address}} {{1.05}}
```
#### View the current wallet's pending transactions:
```shell
hsw-cli pending
```
#### View details about a transaction:
```shell
hsw-cli tx {{transaction_hash}}
```
{% endraw %}