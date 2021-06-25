---
layout: default
title: "openssl dgst"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openssl-dgst">
  <a href="/en/common/openssl-dgst.html">openssl dgst</a> <a href="#openssl-dgst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenSSL command to generate digest values and perform signature operations.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-dgst.html>.

#### Calculate the SHA256 digest for a file, saving the result to a specific file:
```shell
openssl dgst -sha256 -binary -out {{output_file}} {{input_file}}
```
#### Sign a file using an RSA key, saving the result to a specific file:
```shell
openssl dgst -sign {{private_key_file}} -sha256 -sigopt rsa_padding_mode:pss -out {{output_file}} {{input_file}}
```
#### Verify an RSA signature:
```shell
openssl dgst -verify {{public_key_file}} -signature {{signature_file}} -sigopt rsa_padding_mode:pss {{signature_message_file}}
```
#### Sign a file using and ECDSA key:
```shell
openssl dgst -sign {{private_key_file}} -sha256 -out {{output_file}} {{input_file}}
```
#### Verify an ECDSA signature:
```shell
openssl dgst -verify {{public_key_file}} -signature {{signature_file}} {{signature_message_file}}
```
{% endraw %}