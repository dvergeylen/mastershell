---
layout: default
title: "dd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dd">
  <a href="/en/common/dd.html">dd</a> <a href="#dd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert and copy a file.
> More information: <https://www.gnu.org/software/coreutils/dd>.

#### Make a bootable usb drive from an isohybrid file (such like `archlinux-xxx.iso`) and show the progress:
```shell
dd if={{file.iso}} of=/dev/{{usb_drive}} status=progress
```
#### Clone a drive to another drive with 4MB block, ignore error and show progress:
```shell
dd if=/dev/{{source_drive}} of=/dev/{{dest_drive}} bs=4M conv=noerror status=progress
```
#### Generate a file of 100 random bytes by using kernel random driver:
```shell
dd if=/dev/urandom of={{random_file}} bs=100 count=1
```
#### Benchmark the write performance of a disk:
```shell
dd if=/dev/zero of={{file_1GB}} bs=1024 count=1000000
```
#### Generate a system backup into an IMG file and show the progress:
```shell
dd if=/dev/{{drive_device}} of={{path/to/file.img}} status=progress
```
#### Restore a drive from an IMG file and show the progress:
```shell
dd if={{path/to/file.img}} of=/dev/{{drive_device}} status=progress
```
#### Check progress of an ongoing dd operation (Run this command from another shell):
```shell
kill -USR1 $(pgrep ^dd)
```
{% endraw %}