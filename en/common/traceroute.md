---
layout: default
title: "traceroute"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="traceroute">
  <a href="/en/common/traceroute.html">traceroute</a> <a href="#traceroute"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the route packets trace to network host.

#### Traceroute to a host:
```shell
traceroute {{host}}
```
#### Disable IP address and host name mapping:
```shell
traceroute -n {{host}}
```
#### Specify wait time for response:
```shell
traceroute -w {{0.5}} {{host}}
```
#### Specify number of queries per hop:
```shell
traceroute -q {{5}} {{host}}
```
#### Specify size in bytes of probing packet:
```shell
traceroute {{host}} {{42}}
```
{% endraw %}