---
layout: default
title: "cryfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cryfs">
  <a href="/en/common/cryfs.html">cryfs</a> <a href="#cryfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A cryptographic filesystem for the cloud.
> More information: <https://www.cryfs.org/>.

#### Mount an encrypted filesystem. The initialization wizard will be started on the first execution:
```shell
cryfs {{path/to/cipher_dir}} {{path/to/mount_point}}
```
#### Unmount an encrypted filesystem:
```shell
cryfs-unmount {{path/to/mount_point}}
```
#### Automatically unmount after ten minutes of inactivity:
```shell
cryfs --unmount-idle {{10}} {{path/to/cipher_dir}} {{path/to/mount_point}}
```
#### Show a list of supported ciphers:
```shell
cryfs --show-ciphers
```
{% endraw %}