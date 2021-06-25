---
layout: default
title: "ogrinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ogrinfo">
  <a href="/en/common/ogrinfo.html">ogrinfo</a> <a href="#ogrinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List information about an OGR-supported data source.
> More information: <https://gdal.org/programs/ogrinfo.html>.

#### List layers of a GeoPackage:
```shell
ogrinfo {{input}}.gpkg
```
#### Get detailed information about a specific layer of a GeoPackage:
```shell
ogrinfo {{input}}.gpkg {{layer_name}}
```
#### Only show summary information about a specific layer of a GeoPackage:
```shell
ogrinfo -so {{input}}.gpkg {{layer_name}}
```
{% endraw %}