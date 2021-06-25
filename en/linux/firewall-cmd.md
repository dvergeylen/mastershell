---
layout: default
title: "firewall-cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="firewall-cmd">
  <a href="/en/linux/firewall-cmd.html">firewall-cmd</a> <a href="#firewall-cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The firewalld command-line client.

#### View the available firewall zones:
```shell
firewall-cmd --get-active-zones
```
#### View the rules which are currently applied:
```shell
firewall-cmd --list-all
```
#### Permanently move the interface into the block zone, effectively blocking all communication:
```shell
firewall-cmd --permanent --zone={{block}} --change-interface={{enp1s0}}
```
#### Permanently open the port for a service in the specified zone (like port 443 when in the `public` zone):
```shell
firewall-cmd --permanent --zone={{public}} --add-service={{https}}
```
#### Permanently close the port for a service in the specified zone (like port 80 when in the `public` zone):
```shell
firewall-cmd --permanent --zone={{public}} --remove-service={{http}}
```
#### Permanently open two arbitrary ports in the specified zone:
```shell
firewall-cmd --permanent --zone={{public}} --add-port={{25565/tcp}} --add-port={{19132/udp}}
```
#### Reload firewalld to force rule changes to take effect:
```shell
firewall-cmd --reload
```
{% endraw %}