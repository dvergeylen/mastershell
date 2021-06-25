---
layout: default
title: "psping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="psping">
  <a href="/en/windows/psping.html">psping</a> <a href="#psping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A ping tool that includes TCP ping, latency and bandwidth measurement.
> More information: <https://docs.microsoft.com/sysinternals/downloads/psping>.

#### Ping a host using ICMP:
```shell
psping {{hostname}}
```
#### Ping a host over a TCP port:
```shell
psping {{hostname}}:{{port}}
```
#### Specify the number of pings and perform it quietly:
```shell
psping {{hostname}} -n {{pings}} -q
```
#### Ping the target over TCP 50 times and produce a histogram of the results:
```shell
psping {{hostname}}:{{port}} -q -n {{50}} -h
```
#### Display usage information:
```shell
psping /?
```
{% endraw %}