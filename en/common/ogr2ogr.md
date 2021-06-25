---
layout: default
title: "ogr2ogr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ogr2ogr">
  <a href="/en/common/ogr2ogr.html">ogr2ogr</a> <a href="#ogr2ogr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert Simple Features data between file formats.
> More information: <https://gdal.org/programs/ogr2ogr.html#ogr2ogr>.

#### Convert a Shapefile into a GeoPackage:
```shell
ogr2ogr -f GPKG {{output}}.gpkg {{input}}.shp
```
#### Change coordinate reference system of a GeoPackage from `EPSG:4326` to `EPSG:3857`:
```shell
ogr2ogr -s_srs {{EPSG:4326}} -t_srs {{EPSG:3857}} -f GPKG {{output}}.gpkg {{input}}.gpkg
```
#### Convert a CSV file into a GeoPackage, specifying the names of the coordinate columns and assigning a coordinate reference system:
```shell
ogr2ogr -f GPKG {{output}}.gpkg {{input}}.csv -oo X_POSSIBLE_NAMES={{longitude}} -oo Y_POSSIBLE_NAMES={{latitude}} -a_srs {{EPSG:4326}}
```
#### Load a GeoPackage into a PostGIS database:
```shell
ogr2ogr -f "PostgreSQL" PG:dbname="{{database_name}}" {{input}}.gpkg
```
#### Clip layers of a GeoPackage file to the given bounding box:
```shell
ogr2ogr -spat {{min_x}} {{min_y}} {{max_x}} {{max_y}} -f GPKG {{output}}.gpkg {{input}}.gpkg
```
{% endraw %}