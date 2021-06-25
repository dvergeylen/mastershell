---
layout: default
title: "cryptsetup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cryptsetup">
  <a href="/en/linux/cryptsetup.html">cryptsetup</a> <a href="#cryptsetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage plain dm-crypt and LUKS (Linux Unified Key Setup) encrypted volumes.

#### Initialize a LUKS volume (overwrites all data on the partition):
```shell
cryptsetup luksFormat {{/dev/sda1}}
```
#### Open a LUKS volume and create a decrypted mapping at `/dev/mapper/{{target}}`:
```shell
cryptsetup luksOpen {{/dev/sda1}} {{target}}
```
#### Remove an existing mapping:
```shell
cryptsetup luksClose {{target}}
```
#### Change the LUKS volume's passphrase:
```shell
cryptsetup luksChangeKey {{/dev/sda1}}
```
{% endraw %}