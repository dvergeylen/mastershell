---
layout: default
title: "netselect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="netselect">
  <a href="/en/linux/netselect.html">netselect</a> <a href="#netselect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Speed test for choosing a fast network server.
> More information: <https://github.com/apenwarr/netselect>.

#### Choose the server with the lowest latency:
```shell
sudo netselect {{host_1}} {{host_2}}
```
#### Display nameserver resolution and statistics:
```shell
sudo netselect -vv {{host_1}} {{host_2}}
```
#### Define maximum TTL (time to live):
```shell
sudo netselect -m {{10}} {{host_1}} {{host_2}}
```
#### Print fastest N servers among the hosts:
```shell
sudo netselect -s {{N}} {{host_1}} {{host_2}} {{host_3}}
```
#### List available options:
```shell
netselect
```
{% endraw %}