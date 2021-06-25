---
layout: default
title: "stl2gts"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stl2gts">
  <a href="/en/common/stl2gts.html">stl2gts</a> <a href="#stl2gts"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert STL files into the GTS (GNU triangulated surface library) file format.
> More information: <https://manned.org/stl2gts>.

#### Convert an STL file to a GTS file:
```shell
stl2gts < {{path/to/file.stl}} > {{path/to/file.gts}}
```
#### Convert an STL file to a GTS file and revert face normals:
```shell
stl2gts --revert < {{path/to/file.stl}} > {{path/to/file.gts}}
```
#### Convert an STL file to a GTS file and do not merge vertices:
```shell
stl2gts --nomerge < {{path/to/file.stl}} > {{path/to/file.gts}}
```
#### Convert an STL file to a GTS file and display surface statistics:
```shell
stl2gts --verbose < {{path/to/file.stl}} > {{path/to/file.gts}}
```
#### Print help for `stl2gts`:
```shell
stl2gts --help
```
{% endraw %}