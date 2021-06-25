---
layout: default
title: "e2image"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="e2image">
  <a href="/en/linux/e2image.html">e2image</a> <a href="#e2image"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Save critical ext2/ext3/ext4 filesystem metadata to a file.
> More information: <https://manned.org/e2image>.

#### Write metadata located on device to a specific file:
```shell
e2image {{/dev/sdXN}} {{path/to/image_file}}
```
#### Print metadata located on device to stdout:
```shell
e2image {{/dev/sdXN}} -
```
#### Restore the filesystem metadata back to the device:
```shell
e2image -I {{/dev/sdXN}} {{path/to/image_file}}
```
#### Create a large raw sparse file with metadata at proper offsets:
```shell
e2image -r {{/dev/sdXN}} {{path/to/image_file}}
```
#### Create a QCOW2 image file instead of a normal or raw image file:
```shell
e2image -Q {{/dev/sdXN}} {{path/to/image_file}}
```
{% endraw %}