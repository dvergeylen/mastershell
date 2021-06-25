---
layout: default
title: "ssh-keyscan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-keyscan">
  <a href="/de/common/ssh-keyscan.html">ssh-keyscan</a> <a href="#ssh-keyscan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rufe öffentliche SSH Schlüssel eines externen Servers ab.

#### Rufe alle öffentlichen SSH Schlüssel eines Servers ab:
```shell
ssh-keyscan {{server}}
```
#### Rufe alle öffentlichen SSH Schlüssel unter einem bestimmten Port ab:
```shell
ssh-keyscan -p {{port}} {{server}}
```
#### Rufe bestimmte SSH Schüssel-Typen ab:
```shell
ssh-keyscan -t {{rsa,dsa,ecdsa,ed25519}} {{server}}
```
#### Aktualisiere die `known_hosts` SSH Datei mit dem Fingerabdruck eines bestimmten Servers:
```shell
ssh-keyscan -H {{server}} >> ~/.ssh/known_hosts
```
{% endraw %}