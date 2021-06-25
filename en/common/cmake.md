---
layout: default
title: "cmake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmake">
  <a href="/en/common/cmake.html">cmake</a> <a href="#cmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cross-platform build automation system, that generates recipes for native build systems.
> More information: <https://cmake.org/cmake/help/latest/manual/cmake.1.html>.

#### Generate a build recipe in the current directory with `CMakeLists.txt` from a project directory:
```shell
cmake {{path/to/project_directory}}
```
#### Generate a build recipe, with build type set to `Release` with CMake variable:
```shell
cmake {{path/to/project_directory}} -D {{CMAKE_BUILD_TYPE=Release}}
```
#### Use a generated recipe in a given directory to build artifacts:
```shell
cmake --build {{path/to/build_directory}}
```
#### Install the build artifacts into `/usr/local/` and strip debugging symbols:
```shell
cmake --install {{path/to/build_directory}} --strip
```
#### Install the build artifacts using the custom prefix for paths:
```shell
cmake --install {{path/to/build_directory}} --strip --prefix {{path/to/directory}}
```
#### Run a custom build target:
```shell
cmake --build {{path/to/build_directory}} --target {{target_name}}
```
{% endraw %}