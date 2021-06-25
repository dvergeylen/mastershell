---
layout: default
title: "light-arionum-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="light-arionum-cli">
  <a href="/en/common/light-arionum-cli.html">light-arionum-cli</a> <a href="#light-arionum-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The PHP light wallet for the Arionum cryptocurrency.
> More information: <https://github.com/arionum/lightWalletCLI>.

#### Generate a new public/private key pair:
```shell
light-arionum-cli
```
#### Display the balance of the current address:
```shell
light-arionum-cli balance
```
#### Display the balance of the specified address:
```shell
light-arionum-cli balance {{address}}
```
#### Send a transaction with an optional message:
```shell
light-arionum-cli send {{address}} {{value}} {{optional_message}}
```
#### Export the current wallet information:
```shell
light-arionum-cli export
```
#### Display information about the current block:
```shell
light-arionum-cli block
```
#### Display information about the current address' transactions:
```shell
light-arionum-cli transactions
```
#### Display information about a specific transaction:
```shell
light-arionum-cli transaction {{transaction_id}}
```
{% endraw %}