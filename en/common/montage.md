---
layout: default
title: "montage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="montage">
  <a href="/en/common/montage.html">montage</a> <a href="#montage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ImageMagick image montage tool.
> Tiles images into a customisable grid.
> More information: <https://imagemagick.org/script/montage.php>.

#### Tile images into a grid, automatically resizing images larger than the grid cell size:
```shell
montage {{image1.png}} {{image2.jpg}} {{imageN.png}} montage.jpg
```
#### Tile images into a grid, automatically calculating the grid cell size from the largest image:
```shell
montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry +0+0 montage.jpg
```
#### Set the grid cell size and resize images to fit it before tiling:
```shell
montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry 640x480+0+0 montage.jpg
```
#### Limit the number of rows and columns in the grid, causing input images to overflow into multiple output montages:
```shell
montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry +0+0 -tile 2x3 montage_%d.jpg
```
#### Resize and crop images to completely fill their grid cells before tiling:
```shell
montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry +0+0 -resize 640x480^ -gravity center -crop 640x480+0+0 montage.jpg
```
{% endraw %}