---
layout: default
title: "age"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="age">
  <a href="/en/common/age.html">age</a> <a href="#age"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple, modern and secure file encryption tool.
> More information: <https://age-encryption.org>.

#### Generate an encrypted file that can be decrypted with a passphrase:
```shell
age --passphrase --output {{path/to/encrypted_file}} {{path/to/unencrypted_file}}
```
#### Generate a key pair, saving the private key to an unencrypted file and printing the public key to stdout:
```shell
age-keygen --output {{path/to/file}}
```
#### Encrypt a file with one or more public keys that are entered as literals:
```shell
age --recipient {{public_key_1}} --recipient {{public_key_2}} {{path/to/unencrypted_file}} --output {{path/to/encrypted_file}}
```
#### Encrypt a file with one or more public keys that are specified in a recipients file:
```shell
age --recipients-file {{path/to/recipients_file}} {{path/to/unencrypted_file}} --output {{path/to/encrypted_file}}
```
#### Decrypt a file with a passphrase:
```shell
age --decrypt --output {{path/to/decrypted_file}} {{path/to/encrypted_file}}
```
#### Decrypt a file with a private key file:
```shell
age --decrypt --identity {{path/to/private_key_file}} --output {{path/to/decrypted_file}} {{path/to/encrypted_file}}
```
{% endraw %}