---
layout: default
title: "assimp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="assimp">
  <a href="/en/common/assimp.html">assimp</a> <a href="#assimp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line client for the Open Asset Import Library.
> Supports loading of 40+ 3D file formats, and exporting to several popular 3D formats.
> More information: <http://www.assimp.org/>.

#### List all supported import formats:
```shell
assimp listext
```
#### List all supported export formats:
```shell
assimp listexport
```
#### Convert a file to one of the supported output formats, using the default parameters:
```shell
assimp export {{input_file.stl}} {{output_file.obj}}
```
#### Convert a file using custom parameters (the dox_cmd.h file in assimp's source code lists available parameters):
```shell
assimp export {{input_file.stl}} {{output_file.obj}} {{parameters}}
```
#### Display a summary of a 3D file's contents:
```shell
assimp info {{path/to/file}}
```
#### List all supported subcommands ("verbs"):
```shell
assimp help
```
#### Get help on a specific subcommand (e.g. the parameters specific to it):
```shell
assimp {{subcommand}} --help
```
{% endraw %}