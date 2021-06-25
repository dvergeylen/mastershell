---
layout: default
title: "openssl s_client"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-s_client">
  <a href="/en/common/openssl-s_client.html">openssl s_client</a> <a href="#openssl-s_client"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to create TLS client connections.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-s_client.html>.

#### Display the start and expiry dates for a domain's certificate:
```shell
openssl s_client -connect {{host}}:{{port}} 2>/dev/null | openssl x509 -noout -dates
```
#### Display the certificate presented by an SSL/TLS server:
```shell
openssl s_client -connect {{host}}:{{port}} </dev/null
```
#### Display the complete certificate chain of an HTTPS server:
```shell
openssl s_client -connect {{host}}:443 -showcerts </dev/null
```
{% endraw %}