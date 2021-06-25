---
layout: default
title: "josm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="josm">
  <a href="/en/common/josm.html">josm</a> <a href="#josm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extensible OpenStreetMap editor for Java 8+.
> More information: <https://josm.openstreetmap.de/>.

#### Launch JOSM:
```shell
josm
```
#### Launch JOSM in maximized mode:
```shell
josm --maximize
```
#### Launch JOSM and set a specific language:
```shell
josm --language {{de}}
```
#### Launch JOSM and reset all preferences to their default values:
```shell
josm --reset-preferences
```
#### Launch JOSM and download a specific bounding box:
```shell
josm --download {{minlat,minlon,maxlat,maxlon}}
```
#### Launch JOSM and download a specific bounding box as raw GPS:
```shell
josm --downloadgps {{minlat,minlon,maxlat,maxlon}}
```
#### Launch JOSM without plugins:
```shell
josm --skip-plugins
```
{% endraw %}