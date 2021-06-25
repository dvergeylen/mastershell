---
layout: default
title: "jpegoptim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jpegoptim">
  <a href="/en/common/jpegoptim.html">jpegoptim</a> <a href="#jpegoptim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimise JPEG images.
> More information: <https://github.com/tjko/jpegoptim>.

#### Optimise a set of JPEG images, retaining all associated data:
```shell
jpegoptim {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}
```
#### Optimise JPEG images, stripping all non-essential data:
```shell
jpegoptim --strip-all {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}
```
#### Force the output images to be progressive:
```shell
jpegoptim --all-progressive {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}
```
#### Force the output images to have a fixed maximum filesize:
```shell
jpegoptim --size={{250k}} {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}
```
{% endraw %}