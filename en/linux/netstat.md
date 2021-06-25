---
layout: default
title: "netstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="netstat">
  <a href="/en/linux/netstat.html">netstat</a> <a href="#netstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays network-related information such as open connections, open socket ports, etc.
> More information: <https://man7.org/linux/man-pages/man8/netstat.8.html>.

#### List all ports:
```shell
netstat --all
```
#### List all listening ports:
```shell
netstat --listening
```
#### List listening TCP ports:
```shell
netstat --tcp
```
#### Display PID and program names:
```shell
netstat --program
```
#### List information continuously:
```shell
netstat --continuous
```
#### List routes and do not resolve IP addresses to hostnames:
```shell
netstat --route --numeric
```
#### List listening TCP and UDP ports (+ user and process if you're root):
```shell
netstat --listening --program --numeric --tcp --udp --extend
```
{% endraw %}