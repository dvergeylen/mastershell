---
layout: default
title: "nbtscan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nbtscan">
  <a href="/en/common/nbtscan.html">nbtscan</a> <a href="#nbtscan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scan networks for NetBIOS name information.
> More information: <https://github.com/resurrecting-open-source-projects/nbtscan>.

#### Scan a network for NetBIOS names:
```shell
nbtscan {{192.168.0.1/24}}
```
#### Scan a single IP address:
```shell
nbtscan {{192.168.0.1}}
```
#### Display verbose output:
```shell
nbtscan -v {{192.168.0.1/24}}
```
#### Display output in `/etc/hosts` format:
```shell
nbtscan -e {{192.168.0.1/24}}
```
#### Read IP addresses / networks to scan from a file:
```shell
nbtscan -f {{path/to/file.txt}}
```
{% endraw %}