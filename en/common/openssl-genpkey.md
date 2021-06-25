---
layout: default
title: "openssl genpkey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-genpkey">
  <a href="/en/common/openssl-genpkey.html">openssl genpkey</a> <a href="#openssl-genpkey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to generate asymmetric key pairs.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-genpkey.html>.

#### Generate an RSA private key of 2048 bits, saving it to a specific file:
```shell
openssl genpkey -algorithm rsa -pkeyopt rsa_keygen_bits:{{2048}} -out {{filename.key}}
```
#### Generate an elliptic curve private key using the curve `prime256v1`, saving it to a specific file:
```shell
openssl genpkey -algorithm EC -pkeyopt ec_paramgen_curve:{{prime256v1}} -out {{filename.key}}
```
#### Generate an `ED25519` elliptic curve private key, saving it to a specific file:
```shell
openssl genpkey -algorithm {{ED25519}} -out {{filename.key}}
```
{% endraw %}