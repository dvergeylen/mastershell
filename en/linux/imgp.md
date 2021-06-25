---
layout: default
title: "imgp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="imgp">
  <a href="/en/linux/imgp.html">imgp</a> <a href="#imgp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line image resizer and rotator for JPEG and PNG images.

#### Convert single images and/or whole directories containing valid image formats:
```shell
imgp -x {{1366x1000}} {{path/to/directory}} {{path/to/file}}
```
#### Scale an image by 75% and overwrite the source image to a target resolution:
```shell
imgp -x {{75}} -w {{path/to/file}}
```
#### Rotate an image clockwise by 90 degrees:
```shell
imgp -o {{90}} {{path/to/file}}
```
{% endraw %}