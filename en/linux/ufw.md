---
layout: default
title: "ufw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ufw">
  <a href="/en/linux/ufw.html">ufw</a> <a href="#ufw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uncomplicated Firewall.
> Frontend for iptables aiming to make configuration of a firewall easier.
> More information: <https://wiki.ubuntu.com/UncomplicatedFirewall>.

#### Enable ufw:
```shell
ufw enable
```
#### Disable ufw:
```shell
ufw disable
```
#### Show ufw rules, along with their numbers:
```shell
ufw status numbered
```
#### Allow incoming traffic on port 5432 on this host with a comment identifying the service:
```shell
ufw allow {{5432}} comment "{{Service}}"
```
#### Allow only TCP traffic from 192.168.0.4 to any address on this host, on port 22:
```shell
ufw allow proto {{tcp}} from {{192.168.0.4}} to {{any}} port {{22}}
```
#### Deny traffic on port 80 on this host:
```shell
ufw deny {{80}}
```
#### Deny all UDP traffic to port 22:
```shell
ufw deny proto {{udp}} from {{any}} to {{any}} port {{22}}
```
#### Delete a particular rule. The rule number can be retrieved from the `ufw status numbered` command:
```shell
ufw delete {{rule_number}}
```
{% endraw %}