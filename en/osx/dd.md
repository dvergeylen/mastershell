---
layout: default
title: "dd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dd">
  <a href="/en/osx/dd.html">dd</a> <a href="#dd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert and copy a file.

#### Make a bootable usb drive from an isohybrid file (such like `archlinux-xxx.iso`):
```shell
dd if={{file.iso}} of=/dev/{{usb_drive}}
```
#### Clone a drive to another drive with 4MB block and ignore error:
```shell
dd if=/dev/{{source_drive}} of=/dev/{{dest_drive}} bs=4m conv=noerror
```
#### Generate a file of 100 random bytes by using kernel random driver:
```shell
dd if=/dev/urandom of={{random_file}} bs=100 count=1
```
#### Benchmark the write performance of a disk:
```shell
dd if=/dev/zero of={{file_1GB}} bs=1024 count=1000000
```
{% endraw %}