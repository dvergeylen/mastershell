---
layout: default
title: "pngcheck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pngcheck">
  <a href="/en/common/pngcheck.html">pngcheck</a> <a href="#pngcheck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print detailed information about and verify PNG, JNG, and MNG files.
> More information: <http://www.libpng.org/pub/png/apps/pngcheck.html>.

#### Print a summary for an image (width, height, and color depth):
```shell
pngcheck {{image.png}}
```
#### Print information for an image with [c]olorized output:
```shell
pngcheck -c {{image.png}}
```
#### Print [v]erbose information for an image:
```shell
pngcheck -cvt {{image.png}}
```
#### Receive an image from stdin and display detailed information:
```shell
cat {{path/to/image.png}} | pngcheck -cvt
```
#### [s]earch for PNGs within a specific file and display information about them:
```shell
pngcheck -s {{image.png}}
```
#### Search for PNGs within another file and e[x]tract them:
```shell
pngcheck -x {{image.png}}
```
{% endraw %}