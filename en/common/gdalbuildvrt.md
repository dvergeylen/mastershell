---
layout: default
title: "gdalbuildvrt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gdalbuildvrt">
  <a href="/en/common/gdalbuildvrt.html">gdalbuildvrt</a> <a href="#gdalbuildvrt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build Virtual Datasets from a list of existing datasets.
> More information: <https://gdal.org/programs/gdalbuildvrt.html>.

#### Make a virtual mosaic from all TIFF files contained in a directory:
```shell
gdalbuildvrt {{path/to/output.vrt}} {{path/to/input_directory/*.tif}}
```
#### Make a virtual mosaic from files whose name is specified in a text file:
```shell
gdalbuildvrt -input_file_list {{path/to/list.txt}} {{path/to/output.vrt}}
```
#### Make a RGB virtual mosaic from 3 single-band input files:
```shell
gdalbuildvrt -separate {{path/to/rgb.vrt}} {{path/to/red.tif}} {{path/to/green.tif}} {{path/to/blue.tif}}
```
#### Make a virtual mosaic with blue background colour (RGB: 0 0 255):
```shell
gdalbuildvrt -hidenodata -vrtnodata "{{0 0 255}}" {{path/to/output.vrt}} {{path/to/input_directory/*.tif}}
```
{% endraw %}