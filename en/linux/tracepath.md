---
layout: default
title: "tracepath"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tracepath">
  <a href="/en/linux/tracepath.html">tracepath</a> <a href="#tracepath"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trace the path to a network host discovering MTU along this path.
> More information: <https://manned.org/tracepath>.

#### A preferred way to trace the path to a host:
```shell
tracepath -p {{33434}} {{host}}
```
#### Specify the initial destination port, useful with non-standard firewall settings:
```shell
tracepath -p {{destination_port}} {{host}} 
```
#### Print both hostnames and numerical IP addresses:
```shell
tracepath -b {{host}}
```
#### Specify a maximum TTL (number of hops):
```shell
tracepath -m {{max_hops}} {{host}}
```
#### Specify the initial packet length (defaults to 65535 for IPv4 and 128000 for IPv6):
```shell
tracepath -l {{packet_length}} {{host}}
```
#### Use only IPv6 addresses:
```shell
tracepath -6 {{host}}
```
{% endraw %}