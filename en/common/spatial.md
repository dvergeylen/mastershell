---
layout: default
title: "spatial"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="spatial">
  <a href="/en/common/spatial.html">spatial</a> <a href="#spatial"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A set of commands for managing and developing SpatialOS projects.

#### Run this when you use a project for the first time:
```shell
spatial worker build
```
#### Build workers for local deployment on Unity on macOS:
```shell
spatial worker build --target=development --target=Osx
```
#### Build workers for local deployment on Unreal on Windows:
```shell
spatial worker build --target=local --target=Windows
```
#### Deploy locally:
```shell
spatial local launch {{launch_config}} --snapshot={{snapshot_file}}
```
#### Launch a local worker to connect to your local deployment:
```shell
spatial local worker launch {{worker_type}} {{launch_config}}
```
#### Upload an assembly to use for cloud deployments:
```shell
spatial cloud upload {{assembly_name}}
```
#### Launch a cloud deployment:
```shell
spatial cloud launch {{assembly_name}} {{launch_config}} {{deployment_name}}
```
#### Clean worker directories:
```shell
spatial worker clean
```
{% endraw %}