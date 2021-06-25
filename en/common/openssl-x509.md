---
layout: default
title: "openssl x509"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-x509">
  <a href="/en/common/openssl-x509.html">openssl x509</a> <a href="#openssl-x509"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to manage X.509 certificates.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-x509.html>.

#### Display certificate information:
```shell
openssl x509 -in {{filename.crt}} -noout -text
```
#### Display a certificate's expiration date:
```shell
openssl x509 -enddate -noout -in {{filename.pem}}
```
#### Convert a certificate between binary DER encoding and textual PEM encoding:
```shell
openssl x509 -inform {{der}} -outform {{pem}} -in {{original_certificate_file}} -out {{converted_certificate_file}}
```
#### Store a certificate's public key in a file:
```shell
openssl x509 -in {{certificate_file}} -noout -pubkey -out {{output_file}}
```
{% endraw %}