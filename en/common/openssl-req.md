---
layout: default
title: "openssl req"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-req">
  <a href="/en/common/openssl-req.html">openssl req</a> <a href="#openssl-req"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to manage PKCS#10 Certificate Signing Requests.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-req.html>.

#### Generate a certificate signing request to be sent to a certificate authority:
```shell
openssl req -new -sha256 -key {{filename.key}} -out {{filename.csr}}
```
#### Generate a self-signed certificate and a corresponding key-pair, storing both in a file:
```shell
openssl req -new -x509 -newkey {{rsa}}:{{4096}} -keyout {{filename.key}} -out {{filename.cert}} -subj "{{/C=XX/CN=foobar}}" -days {{365}}
```
{% endraw %}