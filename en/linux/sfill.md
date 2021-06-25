---
layout: default
title: "sfill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sfill">
  <a href="/en/linux/sfill.html">sfill</a> <a href="#sfill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Securely overwrite the free space and inodes of the partition where the specified directory resides.
> More information: <https://manned.org/sfill>.

#### Overwrite free space and inodes of a disk with 38 writes (slow but secure):
```shell
sfill {{/path/to/mounted_disk_directory}}
```
#### Overwrite free space and inodes of a disk with 6 writes (fast but less secure) and show status:
```shell
sfill -l -v {{/path/to/mounted_disk_directory}}
```
#### Overwrite free space and inodes of a disk with 1 write (very fast but insecure) and show status:
```shell
sfill -ll -v {{/path/to/mounted_disk_directory}}
```
#### Overwrite only free space of a disk:
```shell
sfill -I {{/path/to/mounted_disk_directory}}
```
#### Overwrite only free inodes of a disk:
```shell
sfill -i {{/path/to/mounted_disk_directory}}
```
{% endraw %}