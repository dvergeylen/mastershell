---
layout: default
title: "bandwhich"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bandwhich">
  <a href="/en/common/bandwhich.html">bandwhich</a> <a href="#bandwhich"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the current network utilization by process, connection or remote IP/hostname.
> More information: <https://github.com/imsnif/bandwhich>.

#### Show the remote addresses table only:
```shell
bandwhich --addresses
```
#### Show DNS queries:
```shell
bandwhich --show-dns
```
#### Show total (cumulative) usage:
```shell
bandwhich --total-utilization
```
#### Show the network utilization for a specific network interface:
```shell
bandwhich --interface {{eth0}}
```
#### Show DNS queries with a given DNS server:
```shell
bandwhich --show-dns --dns-server {{dns_server_ip}}
```
{% endraw %}