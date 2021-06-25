---
layout: default
title: "sshfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sshfs">
  <a href="/en/common/sshfs.html">sshfs</a> <a href="#sshfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Filesystem client based on ssh.
> More information: <https://github.com/libfuse/sshfs>.

#### Mount remote directory:
```shell
sshfs {{username}}@{{remote_host}}:{{remote_directory}} {{mountpoint}}
```
#### Unmount remote directory:
```shell
umount {{mountpoint}}
```
#### Mount remote directory from server with specific port:
```shell
sshfs {{username}}@{{remote_host}}:{{remote_directory}} -p {{2222}}
```
#### Use compression:
```shell
sshfs {{username}}@{{remote_host}}:{{remote_directory}} -C
```
#### Follow symbolic links:
```shell
sshfs -o follow_symlinks {{username}}@{{remote_host}}:{{remote_directory}} {{mountpoint}}
```
{% endraw %}