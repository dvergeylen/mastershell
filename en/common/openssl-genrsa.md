---
layout: default
title: "openssl genrsa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-genrsa">
  <a href="/en/common/openssl-genrsa.html">openssl genrsa</a> <a href="#openssl-genrsa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to generate RSA private keys.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-genrsa.html>.

#### Generate an RSA private key of 2048 bits to stdout:
```shell
openssl genrsa
```
#### Save an RSA private key of an arbitrary number of bits to the output file:
```shell
openssl genrsa -out {{output_file.key}} {{1234}}
```
#### Generate an RSA private key and encrypt it with AES256 (you will be prompted for a passphrase):
```shell
openssl genrsa {{-aes256}}
```
{% endraw %}