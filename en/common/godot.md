---
layout: default
title: "godot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="godot">
  <a href="/en/common/godot.html">godot</a> <a href="#godot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An open source 2D and 3D game engine.
> More information: <https://godotengine.org/>.

#### Run a project if the current directory contains a `project.godot` file, otherwise open the project manager:
```shell
godot
```
#### Edit a project (the current directory must contain a `project.godot` file):
```shell
godot -e
```
#### Open the project manager even if the current directory contains a `project.godot` file:
```shell
godot -p
```
#### Export a project for a given export preset (the preset must be defined in the project):
```shell
godot --export {{preset}} {{output_path}}
```
#### Execute a standalone GDScript file (the script must inherit from `SceneTree` or `MainLoop`):
```shell
godot -s {{script.gd}}
```
{% endraw %}