---
layout: default
title: "ping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ping">
  <a href="/en/osx/ping.html">ping</a> <a href="#ping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send ICMP ECHO_REQUEST packets to network hosts.

#### Ping the specified host:
```shell
ping {{host}}
```
#### Ping a host a specific number of times:
```shell
ping -c {{count}} {{host}}
```
#### Ping `host`, specifying the interval in `seconds` between requests (default is 1 second):
```shell
ping -i {{seconds}} {{host}}
```
#### Ping `host` without trying to lookup symbolic names for addresses:
```shell
ping -n {{host}}
```
#### Ping `host` and ring the bell when a packet is received (if your terminal supports it):
```shell
ping -a {{host}}
```
#### Ping `host` and prints the time a packet was received (this option is an Apple addition):
```shell
ping --apple-time {{host}}
```
{% endraw %}