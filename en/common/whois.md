---
layout: default
title: "whois"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whois">
  <a href="/en/common/whois.html">whois</a> <a href="#whois"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line client for the WHOIS (RFC 3912) protocol.
> More information: <https://github.com/rfc1036/whois>.

#### Get information about a domain name:
```shell
whois {{example.com}}
```
#### Get information about an IP address:
```shell
whois {{8.8.8.8}}
```
#### Get abuse contact for an IP address:
```shell
whois -b {{8.8.8.8}}
```
{% endraw %}