---
layout: default
title: "gpgv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpgv">
  <a href="/en/common/gpgv.html">gpgv</a> <a href="#gpgv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verify OpenPGP signatures.
> More information: <https://www.gnupg.org/documentation/manuals/gnupg/gpgv.html>.

#### Verify a signed file:
```shell
gpgv {{path/to/file}}
```
#### Verify a signed file using a detached signature:
```shell
gpgv {{path/to/signature}} {{path/to/file}}
```
#### Add a file to the list of keyrings (a single exported key also counts as a keyring):
```shell
gpgv --keyring {{./alice.keyring}} {{path/to/signature}} {{path/to/file}}
```
{% endraw %}