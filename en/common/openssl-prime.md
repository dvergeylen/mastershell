---
layout: default
title: "openssl prime"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-prime">
  <a href="/en/common/openssl-prime.html">openssl prime</a> <a href="#openssl-prime"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to compute prime numbers.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-prime.html>.

#### Generate a 2048bit prime number and display it in hexadecimal:
```shell
openssl prime -generate -bits 2048 -hex
```
#### Check if a given number is prime:
```shell
openssl prime {{number}}
```
{% endraw %}