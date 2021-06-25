---
layout: default
title: "svgo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="svgo">
  <a href="/en/common/svgo.html">svgo</a> <a href="#svgo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SVG Optimizer: a Node.js-based tool for optimizing Scalable Vector Graphics files.
> It applies a series of transformation rules (plugins), which can be toggled individually.
> More information: <https://github.com/svg/svgo>.

#### Optimize a file using the default plugins (overwrites the original file):
```shell
svgo {{test.svg}}
```
#### Optimize a file and save the result to another file:
```shell
svgo {{test.svg}} -o {{test.min.svg}}
```
#### Optimize all SVG files within a directory (overwrites the original files):
```shell
svgo -f {{path/to/directory/with/svg/files}}
```
#### Optimize all SVG files within a directory and save the resulting files to another directory:
```shell
svgo -f {{path/to/input/directory}} -o {{path/to/output/directory}}
```
#### Optimize SVG content passed from another command, and save the result to a file:
```shell
{{cat test.svg}} | svgo -i - -o {{test.min.svg}}
```
#### Optimize a file and print out the result:
```shell
svgo {{test.svg}} -o -
```
#### Optimize a file making sure a given plugin is enabled:
```shell
svgo --enable={{plugin_name}}
```
#### Show available plugins:
```shell
svgo --show-plugins
```
{% endraw %}