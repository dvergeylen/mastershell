---
layout: default
title: "encfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="encfs">
  <a href="/en/common/encfs.html">encfs</a> <a href="#encfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mounts or creates encrypted virtual filesystems.
> See also `fusermount`, which can unmount filesystems mounted by this command.
> More information: <https://github.com/vgough/encfs>.

#### Initialize or mount an encrypted filesystem:
```shell
encfs {{/path/to/cipher_dir}} {{/path/to/mount_point}}
```
#### Initialize an encrypted filesystem with standard settings:
```shell
encfs --standard {{/path/to/cipher_dir}} {{/path/to/mount_point}}
```
#### Run encfs in the foreground instead of spawning a daemon:
```shell
encfs -f {{/path/to/cipher_dir}} {{/path/to/mount_point}}
```
#### Mount an encrypted snapshot of a plain directory:
```shell
encfs --reverse {{path/to/plain_dir}} {{path/to/cipher_dir}}
```
{% endraw %}