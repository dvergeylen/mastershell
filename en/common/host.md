---
layout: default
title: "host"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="host">
  <a href="/en/common/host.html">host</a> <a href="#host"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lookup Domain Name Server.

#### Lookup A, AAAA, and MX records of a domain:
```shell
host {{domain}}
```
#### Lookup a field (CNAME, TXT,...) of a domain:
```shell
host -t {{field}} {{domain}}
```
#### Reverse lookup an IP:
```shell
host {{ip_address}}
```
#### Specify an alternate DNS server to query:
```shell
host {{domain}} {{8.8.8.8}}
```
{% endraw %}