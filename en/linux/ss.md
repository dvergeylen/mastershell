---
layout: default
title: "ss"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ss">
  <a href="/en/linux/ss.html">ss</a> <a href="#ss"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to investigate sockets.
> More information: <https://manned.org/ss.8>.

#### Show all TCP/UDP/RAW/UNIX sockets:
```shell
ss -a {{-t|-u|-w|-x}}
```
#### Filter TCP sockets by states, only/exclude:
```shell
ss {{state/exclude}} {{bucket/big/connected/synchronized/...}}
```
#### Show all TCP sockets connected to the local HTTPS port (443):
```shell
ss -t src :{{443}}
```
#### Show all TCP sockets listening on the local 8080 port:
```shell
ss -lt src :{{8080}}
```
#### Show all TCP sockets along with processes connected to a remote ssh port:
```shell
ss -pt dst :{{ssh}}
```
#### Show all UDP sockets connected on specific source and destination ports:
```shell
ss -u 'sport == :{{source_port}} and dport == :{{destination_port}}'
```
#### Show all TCP IPv4 sockets locally connected on the subnet 192.168.0.0/16:
```shell
ss -4t src {{192.168/16}}
```
{% endraw %}