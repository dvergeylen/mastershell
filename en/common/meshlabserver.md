---
layout: default
title: "meshlabserver"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="meshlabserver">
  <a href="/en/common/meshlabserver.html">meshlabserver</a> <a href="#meshlabserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for the MeshLab 3D mesh processing software.

#### Convert an STL file to an OBJ file:
```shell
meshlabserver -i {{input.stl}} -o {{output.obj}}
```
#### Convert a WRL file to a OFF file, including the vertex and face normals in the output mesh:
```shell
meshlabserver -i {{input.wrl}} -o {{output.off}} -om vn fn
```
#### Dump a list of all the available processing filters into a file:
```shell
meshlabserver -d {{filename}}
```
#### Process a 3D file using a filter script created in the MeshLab GUI (Filters > Show current filter script > Save Script):
```shell
meshlabserver -i {{input.ply}} -o {{output.ply}} -s {{filter_script.mlx}}
```
#### Process a 3D file using a filter script, writing the output of the filters into a log file:
```shell
meshlabserver -i {{input.x3d}} -o {{output.x3d}} -s {{filter_script.mlx}} -l {{logfile}}
```
{% endraw %}