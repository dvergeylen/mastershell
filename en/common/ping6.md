---
layout: default
title: "ping6"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ping6">
  <a href="/en/common/ping6.html">ping6</a> <a href="#ping6"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send ICMP ECHO_REQUEST packets to network hosts via IPv6 address.

#### Ping a host:
```shell
ping6 {{host}}
```
#### Ping a host only a specific number of times:
```shell
ping6 -c {{count}} {{host}}
```
#### Ping a host, specifying the interval in seconds between requests (default is 1 second):
```shell
ping6 -i {{seconds}} {{host}}
```
#### Ping a host without trying to lookup symbolic names for addresses:
```shell
ping6 -n {{host}}
```
#### Ping a host and ring the bell when a packet is received (if your terminal supports it):
```shell
ping6 -a {{host}}
```
{% endraw %}