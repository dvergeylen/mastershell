---
layout: default
title: "fls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fls">
  <a href="/en/common/fls.html">fls</a> <a href="#fls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List files and directories in an image file or device.
> More information: <https://wiki.sleuthkit.org/index.php?title=Fls>.

#### Build a recursive fls list over a device, output paths will start with C:
```shell
fls -r -m {{C:}} {{/dev/loop1p1}}
```
#### Analyse a single partition, providing the sector offset at which the filesystem starts in the image:
```shell
fls -r -m {{C:}} -o {{sector}} {{path/to/image_file}}
```
#### Analyse a single partition, providing the timezone of the original system:
```shell
fls -r -m {{C:}} -z {{timezone}} {{/dev/loop1p1}}
```
{% endraw %}