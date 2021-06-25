---
layout: default
title: "nslookup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nslookup">
  <a href="/en/common/nslookup.html">nslookup</a> <a href="#nslookup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query name server(s) for various domain records.

#### Query your system's default name server for an IP address (A record) of the domain:
```shell
nslookup {{example.com}}
```
#### Query a given name server for a NS record of the domain:
```shell
nslookup -type=NS {{example.com}} {{8.8.8.8}}
```
#### Query for a reverse lookup (PTR record) of an IP address:
```shell
nslookup -type=PTR {{54.240.162.118}}
```
#### Query for ANY available records using TCP protocol:
```shell
nslookup -vc -type=ANY {{example.com}} 
```
#### Query a given name server for the whole zone file (zone transfer) of the domain using TCP protocol:
```shell
nslookup -vc -type=AXFR {{example.com}} {{name_server}}
```
#### Query for a mail server (MX record) of the domain, showing details of the transaction:
```shell
nslookup -type=MX -debug {{example.com}}
```
#### Query a given name server on a specific port number for a TXT record of the domain:
```shell
nslookup -port={{port_number}} -type=TXT {{example.com}} {{name_server}}
```
{% endraw %}