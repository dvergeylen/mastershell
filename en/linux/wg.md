---
layout: default
title: "wg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wg">
  <a href="/en/linux/wg.html">wg</a> <a href="#wg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the configuration of WireGuard interfaces.
> More information: <https://www.wireguard.com/quickstart/>.

#### Check status of currently active interfaces:
```shell
sudo wg
```
#### Print a new private key:
```shell
wg genkey
```
#### Print a new public key:
```shell
echo {{private_key}} | wg pubkey
```
#### Generate a public and private key:
```shell
wg genkey | tee {{privatekey.txt}} | wg pubkey > {{publickey.txt}}
```
{% endraw %}