---
layout: default
title: "mmls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mmls">
  <a href="/en/common/mmls.html">mmls</a> <a href="#mmls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the partition layout of a volume system.
> More information: <https://wiki.sleuthkit.org/index.php?title=Mmls>.

#### Display the partition table stored in an image file:
```shell
mmls {{path/to/image_file}}
```
#### Display the partition table with an additional column for the partition size:
```shell
mmls -B -i {{path/to/image_file}}
```
#### Display the partition table in a split EWF image:
```shell
mmls -i ewf {{image.e01}} {{image.e02}}
```
#### Display nested partition tables:
```shell
mmls -t {{nested_table_type}} -o {{offset}} {{path/to/image_file}}
```
{% endraw %}