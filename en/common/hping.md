---
layout: default
title: "hping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hping">
  <a href="/en/common/hping.html">hping</a> <a href="#hping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line oriented TCP/IP packet assembler and analyzer.
> Inspired by the `ping` command.
> More information: <http://www.hping.org>.

#### Ping localhost over TCP:
```shell
hping3 {{localhost}}
```
#### Ping an IP address over TCP on a specific port:
```shell
hping3 -p {{80}} -S {{192.168.1.1}}
```
#### Ping an IP address over UDP on port 80:
```shell
hping3 --udp -p {{80}} -S {{192.168.1.1}}
```
#### Scan a set of TCP ports on a specific IP address:
```shell
hping3 --scan {{80,3000,9000}} -S {{192.168.1.1}}
```
#### Perform a charge test on port 80:
```shell
hping3 --flood -p {{80}} -S {{192.168.1.1}}
```
{% endraw %}