---
layout: default
title: "sxiv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sxiv">
  <a href="/en/linux/sxiv.html">sxiv</a> <a href="#sxiv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple X Image Viewer.
> More information: <https://github.com/muennich/sxiv>.

#### Open an image:
```shell
sxiv {{path/to/file}}
```
#### Open an image in fullscreen mode:
```shell
sxiv -f {{path/to/file}}
```
#### Open a newline-separated list of images, reading filenames from standard input:
```shell
echo {{path/to/file}} | sxiv -i
```
#### Open a space-separated list of images as a slideshow:
```shell
sxiv -S {{seconds}} {{path/to/file}}
```
#### Open a space-separated list of images in thumbnail mode:
```shell
sxiv -t {{path/to/file}}
```
{% endraw %}