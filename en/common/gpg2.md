---
layout: default
title: "gpg2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg2">
  <a href="/en/common/gpg2.html">gpg2</a> <a href="#gpg2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard 2.
> See `gpg` for GNU Privacy Guard 1.
> More information: <https://docs.releng.linuxfoundation.org/en/latest/gpg.html>.

#### List imported keys:
```shell
gpg2 --list-keys
```
#### Encrypt a specified file for a specified recipient, writing the output to a new file with `.gpg` appended:
```shell
gpg2 --encrypt --recipient {{alice@example.com}} {{path/to/doc.txt}}
```
#### Encrypt a specified file with only a passphrase, writing the output to a new file with `.gpg` appended:
```shell
gpg2 --symmetric {{path/to/doc.txt}}
```
#### Decrypt a specified file, writing the result to the standard output:
```shell
gpg2 --decrypt {{path/to/doc.txt.gpg}}
```
#### Import a public key:
```shell
gpg2 --import {{path/to/public_key.gpg}}
```
#### Export the public key of a specified email address to the standard output:
```shell
gpg2 --export --armor {{alice@example.com}}
```
#### Export the private key with a specified email address to the standard output:
```shell
gpg2 --export-secret-keys --armor {{alice@example.com}}
```
{% endraw %}