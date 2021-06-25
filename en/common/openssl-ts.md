---
layout: default
title: "openssl ts"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-ts">
  <a href="/en/common/openssl-ts.html">openssl ts</a> <a href="#openssl-ts"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to generate and verify timestamps.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-ts.html>.

#### Generate a SHA-512 timestamp request of a specific file and output to `file.tsq`:
```shell
openssl ts -query -data {{path/to/file}} -sha512 -out {{path/to/file.tsq}}
```
#### Check the date and metadata of a specific timestamp response file:
```shell
openssl ts -reply -in {{path/to/file.tsr}} -text
```
#### Verify a timestamp request file and a timestamp response file from the server with an SSL certificate file:
```shell
openssl ts -verify -in {{path/to/file.tsr}} -queryfile {{path/to/file.tsq}} -partial_chain -CAfile {{path/to/cert.pem}}
```
#### Create a timestamp response for request using key and signing certificate and output it to `file.tsr`:
```shell
openssl ts -reply -queryfile {{path/to/file.tsq}} -inkey {{path/to/tsakey.pem}} -signer tsacert.pem -out {{path/to/file.tsr}}
```
{% endraw %}