---
layout: default
title: "drill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drill">
  <a href="/en/common/drill.html">drill</a> <a href="#drill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform various DNS queries.
> More information: <https://manned.org/drill>.

#### Lookup the IP(s) associated with a hostname (A records):
```shell
drill {{example.com}}
```
#### Lookup the mail server(s) associated with a given domain name (MX record):
```shell
drill mx {{example.com}}
```
#### Get all types of records for a given domain name:
```shell
drill any {{example.com}}
```
#### Specify an alternate DNS server to query:
```shell
drill {{example.com}} @{{8.8.8.8}}
```
#### Perform a reverse DNS lookup on an IP address (PTR record):
```shell
drill -x {{8.8.8.8}}
```
#### Perform DNSSEC trace from root servers down to a domain name:
```shell
drill -TD {{example.com}}
```
#### Show DNSKEY record(s) for a domain name:
```shell
drill -s dnskey {{example.com}}
```
{% endraw %}