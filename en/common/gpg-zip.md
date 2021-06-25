---
layout: default
title: "gpg-zip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg-zip">
  <a href="/en/common/gpg-zip.html">gpg-zip</a> <a href="#gpg-zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encrypt files and directories in an archive using GPG.
> More information: <https://www.gnupg.org/documentation/manuals/gnupg/gpg_002dzip.html>.

#### Encrypt a directory into `archive.gpg` using a passphrase:
```shell
gpg-zip --symmetric --output {{archive.gpg}} {{path/to/directory}}
```
#### Decrypt `archive.gpg` into a directory of the same name:
```shell
gpg-zip --decrypt {{path/to/archive.gpg}}
```
#### List the contents of the encrypted `archive.gpg`:
```shell
gpg-zip --list-archive {{path/to/archive.gpg}}
```
{% endraw %}