---
layout: default
title: "hdiutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hdiutil">
  <a href="/en/osx/hdiutil.html">hdiutil</a> <a href="#hdiutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to create and manage disk images.

#### Mount an image:
```shell
hdiutil attach {{path/to/image_file}}
```
#### Unmount an image:
```shell
hdiutil detach /Volumes/{{volume_name}}
```
#### List mounted images:
```shell
hdiutil info
```
#### Create an ISO image from the contents of a directory:
```shell
hdiutil makehybrid -o {{path/to/output_file}} {{path/to/directory}}
```
{% endraw %}