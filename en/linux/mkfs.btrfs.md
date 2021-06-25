---
layout: default
title: "mkfs.btrfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs.btrfs">
  <a href="/en/linux/mkfs.btrfs.html">mkfs.btrfs</a> <a href="#mkfs.btrfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a btrfs filesystem.
> Defaults to `raid1`, which specifies 2 copies of a given data block spread across 2 different devices.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/mkfs.btrfs>.

#### Create a btrfs filesystem on a single device:
```shell
sudo mkfs.btrfs --metadata single --data single {{/dev/sda}}
```
#### Create a btrfs filesystem on multiple devices with raid1:
```shell
sudo mkfs.btrfs --metadata raid1 --data raid1 {{/dev/sda}} {{/dev/sdb}} {{/dev/sdN}}
```
#### Set a label for the filesystem:
```shell
sudo mkfs.btrfs --label "{{label}}" {{/dev/sda}} [{{/dev/sdN}}]
```
{% endraw %}