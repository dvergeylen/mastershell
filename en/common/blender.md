---
layout: default
title: "blender"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="blender">
  <a href="/en/common/blender.html">blender</a> <a href="#blender"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface to the Blender 3D computer graphics application.
> Arguments are executed in the order they are given.
> More information: <https://docs.blender.org/manual/en/latest/render/workflows/command_line.html>.

#### Render all frames of an animation in the background, without loading the UI (output is saved to `/tmp`):
```shell
blender -b {{filename}}.blend -a
```
#### Render an animation using a specific image naming pattern, in a path relative (`//`) to the .blend file:
```shell
blender -b {{filename}}.blend -o //{{render/frame_###.png}} -a
```
#### Render the 10th frame of an animation as a single image, saved to an existing directory (absolute path):
```shell
blender -b {{filename}}.blend -o {{/path/to/output_directory}} -f {{10}}
```
#### Render the second last frame in an animation as a JPEG image, saved to an existing directory (relative path):
```shell
blender -b {{filename}}.blend -o //{{output_directory}} -F {{JPEG}} -f {{-2}}
```
#### Render the animation of a specific scene, starting at frame 10 and ending at frame 500:
```shell
blender -b {{filename}}.blend -S {{scene_name}} -s {{10}} -e {{500}} -a
```
#### Render an animation at a specific resolution, by passing a Python expression:
```shell
blender -b {{filename}}.blend --python-expr '{{import bpy; bpy.data.scenes[0].render.resolution_percentage = 25}}' -a
```
#### Start an interactive Blender session in the terminal with a python console (do `import bpy` after starting):
```shell
blender -b --python-console
```
{% endraw %}