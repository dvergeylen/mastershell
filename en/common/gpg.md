---
layout: default
title: "gpg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg">
  <a href="/en/common/gpg.html">gpg</a> <a href="#gpg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard.
> See `gpg2` for GNU Privacy Guard 2.
> More information: <https://gnupg.org>.

#### Sign `doc.txt` without encryption (writes output to `doc.txt.asc`):
```shell
gpg --clearsign {{doc.txt}}
```
#### Encrypt `doc.txt` for alice@example.com (output to `doc.txt.gpg`):
```shell
gpg --encrypt --recipient {{alice@example.com}} {{doc.txt}}
```
#### Encrypt `doc.txt` with only a passphrase (output to `doc.txt.gpg`):
```shell
gpg --symmetric {{doc.txt}}
```
#### Decrypt `doc.txt.gpg` (output to stdout):
```shell
gpg --decrypt {{doc.txt.gpg}}
```
#### Import a public key:
```shell
gpg --import {{public.gpg}}
```
#### Export public key for alice@example.com (output to stdout):
```shell
gpg --export --armor {{alice@example.com}}
```
#### Export private key for alice@example.com (output to stdout):
```shell
gpg --export-secret-keys --armor {{alice@example.com}}
```
{% endraw %}