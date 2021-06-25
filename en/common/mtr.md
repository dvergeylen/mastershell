---
layout: default
title: "mtr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mtr">
  <a href="/en/common/mtr.html">mtr</a> <a href="#mtr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Matt's Traceroute: combined traceroute and ping tool.
> More information: <https://bitwizard.nl/mtr>.

#### Traceroute to a host and continuously ping all intermediary hops:
```shell
mtr {{host}}
```
#### Disable IP address and host name mapping:
```shell
mtr -n {{host}}
```
#### Generate output after pinging each hop 10 times:
```shell
mtr -w {{host}}
```
#### Force IP IPv4 or IPV6:
```shell
mtr -4 {{host}}
```
#### Wait for a given time (in seconds) before sending another packet to the same hop:
```shell
mtr -i {{seconds}} {{host}}
```
{% endraw %}