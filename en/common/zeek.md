---
layout: default
title: "zeek"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zeek">
  <a href="/en/common/zeek.html">zeek</a> <a href="#zeek"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Passive network traffic analyser.
> Any output and log files will be saved to the current working directory.
> More information: <https://docs.zeek.org/en/lts/quickstart.html#zeek-as-a-command-line-utility>.

#### Analyze live traffic from a network interface:
```shell
sudo zeek --iface {{interface}}
```
#### Analyze live traffic from a network interface and load custom scripts:
```shell
sudo zeek --iface {{interface}} {{script1}} {{script2}}
```
#### Analyze live traffic from a network interface, without loading any scripts:
```shell
sudo zeek --bare-mode --iface {{interface}}
```
#### Analyze live traffic from a network interface, applying a `tcpdump` filter:
```shell
sudo zeek --filter {{path/to/filter}} --iface {{interface}}
```
#### Analyze live traffic from a network interface using a watchdog timer:
```shell
sudo zeek --watchdog --iface {{interface}}
```
#### Analyze traffic from a `pcap` file:
```shell
zeek --readfile {{path/to/file.trace}}
```
{% endraw %}