---
layout: default
title: "telnet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="telnet">
  <a href="/en/common/telnet.html">telnet</a> <a href="#telnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Connect to a specified port of a host using the telnet protocol.

#### Telnet to the default port of a host:
```shell
telnet {{host}}
```
#### Telnet to a specific port of a host:
```shell
telnet {{ip_address}} {{port}}
```
#### Exit a telnet session:
```shell
quit
```
#### Emit the default escape character combination for terminating the session:
```shell
Ctrl + ]
```
#### Start telnet with "x" as the session termination character:
```shell
telnet -e {{x}} {{ip_address}} {{port}}
```
#### Telnet to Star Wars animation:
```shell
telnet {{towel.blinkenlights.nl}}
```
{% endraw %}