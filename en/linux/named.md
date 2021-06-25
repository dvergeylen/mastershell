---
layout: default
title: "named"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="named">
  <a href="/en/linux/named.html">named</a> <a href="#named"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute the DNS (Dynamic Name Service) server daemon that converts host names to IP addresses and vice versa.
> More information: <https://manned.org/named>.

#### Read the default configuration file `/etc/named.conf`, read any initial data and listen for queries:
```shell
named
```
#### Read a custom configuration file:
```shell
named -c {{path/to/named.conf}}
```
#### Use IPv4 or IPv6 only, even if the host machine is capable of utilising other protocols:
```shell
named {{-4|-6}}
```
#### Listen for queries on a specific port instead of the default port 53:
```shell
named -p {{port}}
```
#### Run the server in the foreground and do not daemonize:
```shell
named -f
```
{% endraw %}