---
layout: default
title: "hping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hping">
  <a href="/fr/common/hping.html">hping</a> <a href="#hping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil en ligne de commande permettant d'assembler ou analyser des paquets TCP/IP.
> Inspirer par la commande `ping`.
> Plus d'informations : <http://www.hping.org>.

#### Ping localhost via TCP :
```shell
hping3 {{localhost}}
```
#### Ping une adresse IP, via TCP, sur un port spécifique :
```shell
hping3 -p {{80}} -S {{192.168.1.1}}
```
#### Ping une adresse IP, via UDP, sur le port 80 :
```shell
hping3 --udp -p {{80}} -S {{192.168.1.1}}
```
#### Scanner un ensemble de ports TCP, sur une adresse IP spécifique :
```shell
hping3 --scan {{80,3000,9000}} -S {{192.168.1.1}}
```
#### Effectuer un test de montée en charge sur le port 80 :
```shell
hping3 --flood -p {{80}} -S {{192.168.1.1}}
```
{% endraw %}