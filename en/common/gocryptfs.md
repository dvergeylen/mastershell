---
layout: default
title: "gocryptfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gocryptfs">
  <a href="/en/common/gocryptfs.html">gocryptfs</a> <a href="#gocryptfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encrypted overlay filesystem written in Go.
> More information: <https://github.com/rfjakob/gocryptfs>.

#### Initialize an encrypted filesystem:
```shell
gocryptfs -init {{path/to/cipher_dir}}
```
#### Mount an encrypted filesystem:
```shell
gocryptfs {{path/to/cipher_dir}} {{path/to/mount_point}}
```
#### Mount with the explicit master key instead of password:
```shell
gocryptfs --masterkey {{path/to/cipher_dir}} {{path/to/mount_point}}
```
#### Change the password:
```shell
gocryptfs --passwd {{path/to/cipher_dir}}
```
#### Make an encrypted snapshot of a plain directory:
```shell
gocryptfs --reverse {{path/to/plain_dir}} {{path/to/cipher_dir}}
```
{% endraw %}