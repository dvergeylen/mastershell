---
layout: default
title: "meson"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="meson">
  <a href="/en/common/meson.html">meson</a> <a href="#meson"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SCons-like build system that uses python as a front-end language and Ninja as a building backend.
> More information: <https://mesonbuild.com>.

#### Generate a c project with a given name and version:
```shell
meson init --language={{c}} --name={{myproject}} --version={{0.1}}
```
#### Configure the `builddir` with default values:
```shell
meson setup {{build_dir}}
```
#### Build the project:
```shell
meson compile -C {{path/to/build_dir}}
```
#### Show the help:
```shell
meson --help
```
#### Show version info:
```shell
meson --version
```
{% endraw %}