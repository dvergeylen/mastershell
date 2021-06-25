---
layout: default
title: "mogrify"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mogrify">
  <a href="/en/common/mogrify.html">mogrify</a> <a href="#mogrify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform operations on multiple images, such as resizing, cropping, flipping, and adding effects.
> Changes are applied directly to the original file.
> More information: <https://imagemagick.org/script/mogrify.php>.

#### Resize all JPEG images in the directory to 50% of their initial size:
```shell
mogrify -resize {{50%}} {{*.jpg}}
```
#### Resize all images starting with "DSC" to 800x600:
```shell
mogrify -resize {{800x600}} {{DSC*}}
```
#### Convert all PNG images in the directory to JPEG:
```shell
mogrify -format {{jpg}} {{*.png}}
```
#### Halve the saturation of all image files in the current directory:
```shell
mogrify -modulate {{100,50}} {{*}}
```
#### Double the brightness of all image files in the current directory:
```shell
mogrify -modulate {{200}} {{*}}
```
{% endraw %}