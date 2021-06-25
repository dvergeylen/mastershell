---
layout: default
title: "nft"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nft">
  <a href="/en/linux/nft.html">nft</a> <a href="#nft"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Allows configuration of tables, chains and rules provided by the Linux kernel firewall.
> Nftables replaces iptables.

#### View current configuration:
```shell
sudo nft list ruleset
```
#### Add a new table with family "inet" and table "filter":
```shell
sudo nft add table {{inet}} {{filter}}
```
#### Add a new chain to accept all inbound traffic:
```shell
sudo nft add chain {{inet}} {{filter}} {{input}} \{ type {{filter}} hook {{input}} priority {{0}} \; policy {{accept}} \}
```
#### Add a new rule to accept several TCP ports:
```shell
sudo nft add rule {{inet}} {{filter}} {{input}} {{tcp}} {{dport \{ telnet, ssh, http, https \} accept}}
```
#### Show rule handles:
```shell
sudo nft --handle --numeric list chain {{family}} {{table}} {{chain}}
```
#### Delete a rule:
```shell
sudo nft delete rule {{inet}} {{filter}} {{input}} handle {{3}}
```
#### Save current configuration:
```shell
sudo nft list ruleset > {{/etc/nftables.conf}}
```
{% endraw %}