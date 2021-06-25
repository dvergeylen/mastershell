---
layout: default
title: "dig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dig">
  <a href="/en/common/dig.html">dig</a> <a href="#dig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DNS Lookup utility.
> More information: <https://manpages.debian.org/dnsutils/dig.1.html>.

#### Lookup the IP(s) associated with a hostname (A records):
```shell
dig +short {{example.com}}
```
#### Get a detailed answer for a given domain (A records):
```shell
dig +noall +answer {{example.com}}
```
#### Query a specific DNS record type associated with a given domain name:
```shell
dig +short {{example.com}} {{A|MX|TXT|CNAME|NS}}
```
#### Get all types of records for a given domain name:
```shell
dig {{example.com}} ANY
```
#### Specify an alternate DNS server to query:
```shell
dig @{{8.8.8.8}} {{example.com}}
```
#### Perform a reverse DNS lookup on an IP address (PTR record):
```shell
dig -x {{8.8.8.8}}
```
#### Find authoritative name servers for the zone and display SOA records:
```shell
dig +nssearch {{example.com}}
```
#### Perform iterative queries and display the entire trace path to resolve a domain name:
```shell
dig +trace {{example.com}}
```
{% endraw %}