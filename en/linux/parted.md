---
layout: default
title: "parted"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="parted">
  <a href="/en/linux/parted.html">parted</a> <a href="#parted"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A partition manipulation program.
> See also: `partprobe`.
> More information: <https://www.gnu.org/software/parted/parted.html>.

#### List partitions on all block devices:
```shell
sudo parted --list
```
#### Start interactive mode with the specified disk selected:
```shell
sudo parted {{/dev/sdX}}
```
#### Create a new partition table of the specified label-type:
```shell
sudo parted --script {{/dev/sdX}} mklabel {{aix|amiga|bsd|dvh|gpt|loop|mac|msdos|pc98|sun}}
```
#### Show partition information in interactive mode:
```shell
print
```
#### Select a disk in interactive mode:
```shell
select {{/dev/sdX}}
```
#### Create a 16GB partition with the specified filesystem in interactive mode:
```shell
mkpart {{primary|logical|extended}} {{btrfs|ext2|ext3|ext4|fat16|fat32|hfs|hfs+|linux-swap|ntfs|reiserfs|udf|xfs}} {{0%}} {{16G}}
```
#### Resize a partition in interactive mode:
```shell
resizepart {{/dev/sdXN}} {{end_position_of_partition}}
```
#### Remove a partition in interactive mode:
```shell
rm {{/dev/sdXN}}
```
{% endraw %}