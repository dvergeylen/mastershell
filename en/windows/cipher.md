---
layout: default
title: "cipher"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cipher">
  <a href="/en/windows/cipher.html">cipher</a> <a href="#cipher"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encrypt or decrypt files on NTFS drives.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cipher>.

#### Encrypt a file or directory:
```shell
cipher /e:{{path/to/file_or_directory}}
```
#### Decrypt a file or directory:
```shell
cipher /d:{{path/to/file_or_directory}}
```
#### Securely remove a file or directory:
```shell
cipher /w:{{path/to/file_or_directory}}
```
{% endraw %}