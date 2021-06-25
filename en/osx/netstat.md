---
layout: default
title: "netstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="netstat">
  <a href="/en/osx/netstat.html">netstat</a> <a href="#netstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays network-related information such as open connections, open socket ports, etc.
> More information: <https://www.unix.com/man-page/osx/1/netstat>.

#### List all ports:
```shell
netstat -a
```
#### List all listening ports:
```shell
netstat -l
```
#### List listening TCP ports:
```shell
netstat -t
```
#### Display PID and program names for a specific protocol:
```shell
netstat -p {{protocol}}
```
#### Print the routing table:
```shell
netstat -nr
```
{% endraw %}