---
layout: default
title: "minisign"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minisign">
  <a href="/en/common/minisign.html">minisign</a> <a href="#minisign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A dead simple tool to sign files and verify signatures.
> More information: <https://jedisct1.github.io/minisign/>.

#### Generate a new keypair at the default location:
```shell
minisign -G
```
#### Sign a file:
```shell
minisign -Sm {{path/to/file}}
```
#### Sign a file, adding a trusted (signed) and an untrusted (unsigned) comment in the signature:
```shell
minisign -Sm {{path/to/file}} -c "{{Untrusted comment}}" -t "{{Trusted comment}}"
```
#### Verify a file and the trusted comments in its signature using the specified public key file:
```shell
minisign -Vm {{path/to/file}} -p {{path/to/publickey.pub}}
```
#### Verify a file and the trusted comments in its signature, specifying a public key as a Base64 encoded literal:
```shell
minisign -Vm {{path/to/file}} -P "{{public_key_base64}}"
```
{% endraw %}