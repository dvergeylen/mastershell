---
layout: default
title: "tcptraceroute"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tcptraceroute">
  <a href="/en/linux/tcptraceroute.html">tcptraceroute</a> <a href="#tcptraceroute"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A traceroute implementation using TCP packets.
> More information: <https://github.com/mct/tcptraceroute>.

#### Trace the route to a host:
```shell
tcptraceroute {{host}}
```
#### Specify the destination port and packet length in bytes:
```shell
tcptraceroute {{host}} {{destination_port}} {{packet_length}}
```
#### Specify the local source port and source address:
```shell
tcptraceroute {{host}} -p {{source_port}} -s {{source_address}}
```
#### Set the first and maximum TTL:
```shell
tcptraceroute {{host}} -f {{first_ttl}} -m {{max_ttl}}
```
#### Specify the wait time and number of queries per hop:
```shell
tcptraceroute {{host}} -w {{wait_time}} -q {{number_of_queries}}
```
#### Specify the interface:
```shell
tcptraceroute {{host}} -i {{interface}}
```
{% endraw %}