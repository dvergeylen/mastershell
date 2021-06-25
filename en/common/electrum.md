---
layout: default
title: "electrum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="electrum">
  <a href="/en/common/electrum.html">electrum</a> <a href="#electrum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ergonomic Bitcoin wallet and private key management.
> More information: <https://electrum.org>.

#### Create a new wallet:
```shell
electrum -w {{new_wallet.dat}} create
```
#### Restore an existing wallet from seed offline:
```shell
electrum -w {{recovery_wallet.dat}} restore -o
```
#### Create a signed transaction offline:
```shell
electrum mktx {{recipient}} {{amount}} -f 0.0000001 -F {{from}} -o
```
#### Display all wallet receiving addresses:
```shell
electrum listaddresses -a
```
#### Sign a message:
```shell
electrum signmessage {{address}} {{message}}
```
#### Verify a message:
```shell
electrum verifymessage {{address}} {{signature}} {{message}}
```
#### Connect only to a specific electrum-server instance:
```shell
electrum -p socks5:{{127.0.0.1}}:9050 -s {{56ckl5obj37gypcu.onion}}:50001:t -1
```
{% endraw %}