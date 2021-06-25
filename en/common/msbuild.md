---
layout: default
title: "msbuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="msbuild">
  <a href="/en/common/msbuild.html">msbuild</a> <a href="#msbuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Microsoft build tool for Visual Studio project solutions.
> More information: <https://docs.microsoft.com/visualstudio/msbuild>.

#### Build the first project file in the current directory:
```shell
msbuild
```
#### Build a specific project file:
```shell
msbuild {{path/to/project_file}}
```
#### Set one or more semicolon-separated targets to build:
```shell
msbuild {{path/to/project_file}} /target:{{targets}}
```
#### Set one or more semicolon-separated properties:
```shell
msbuild {{path/to/project_file}} /property:{{name=value}}
```
#### Set the build tools version to use:
```shell
msbuild {{path/to/project_file}} /toolsversion:{{version}}
```
#### Display detailed information at the end of the log about how the project was configured:
```shell
msbuild {{path/to/project_file}} /detailedsummary
```
#### Display detailed help information:
```shell
msbuild /help
```
{% endraw %}