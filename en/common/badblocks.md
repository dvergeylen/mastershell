---
layout: default
title: "badblocks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="badblocks">
  <a href="/en/common/badblocks.html">badblocks</a> <a href="#badblocks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search a device for bad blocks.
> Some usages of badblocks can cause destructive actions, such as erasing all data on a disk, including the partition table.
> More information: <https://manned.org/badblocks>.

#### Search a disk for bad blocks by using a non-destructive read-only test:
```shell
sudo badblocks {{/dev/sdX}}
```
#### Search an unmounted disk for bad blocks with a non-destructive read-write test:
```shell
sudo badblocks -n {{/dev/sdX}}
```
#### Search an unmounted disk for bad blocks with a destructive write test:
```shell
sudo badblocks -w {{/dev/sdX}}
```
#### Search an unmounted disk for bad blocks with a destructive write test and show verbose status:
```shell
sudo badblocks -svw {{/dev/sdX}}
```
#### Search an unmounted disk in destructive mode and output found blocks to a file:
```shell
sudo badblocks -o {{path/to/file}} -w {{/dev/sdX}}
```
#### Search an unmounted disk in destructive mode with improved speed using 4K block size and 64K block count:
```shell
sudo badblocks -w -b {{4096}} -c {{65536}} {{/dev/sdX}}
```
{% endraw %}