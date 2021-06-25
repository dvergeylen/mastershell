---
layout: default
title: "tcpdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tcpdump">
  <a href="/en/common/tcpdump.html">tcpdump</a> <a href="#tcpdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dump traffic on a network.
> More information: <https://www.tcpdump.org>.

#### List available network interfaces:
```shell
tcpdump -D
```
#### Capture the traffic of a specific interface:
```shell
tcpdump -i {{eth0}}
```
#### Capture all TCP traffic showing contents (ASCII) in console:
```shell
tcpdump -A tcp
```
#### Capture the traffic from or to a host:
```shell
tcpdump host {{www.example.com}}
```
#### Capture the traffic from a specific interface, source, destination and destination port:
```shell
tcpdump -i {{eth0}} src {{192.168.1.1}} and dst {{192.168.1.2}} and dst port {{80}}
```
#### Capture the traffic of a network:
```shell
tcpdump net {{192.168.1.0/24}}
```
#### Capture all traffic except traffic over port 22 and save to a dump file:
```shell
tcpdump -w {{dumpfile.pcap}} port not {{22}}
```
#### Read from a given dump file:
```shell
tcpdump -r {{dumpfile.pcap}}
```
{% endraw %}