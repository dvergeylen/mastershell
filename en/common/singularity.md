---
layout: default
title: "singularity"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="singularity">
  <a href="/en/common/singularity.html">singularity</a> <a href="#singularity"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Singularity containers and images.

#### Download a remote image from Sylabs Cloud:
```shell
singularity pull --name {{image.sif}} {{library://godlovedc/funny/lolcow:latest}}
```
#### Rebuild a remote image using latest Singularity image format:
```shell
singularity build {{image.sif}} {{docker://godlovedc/lolcow}}
```
#### Start a container from an image and get a shell inside of it:
```shell
singularity shell {{image.sif}}
```
#### Start a container from an image and run a command:
```shell
singularity exec {{image.sif}} {{command}}
```
#### Start a container from an image and execute the internal runscript:
```shell
singularity run {{image.sif}}
```
#### Build a singularity image from a recipe file:
```shell
sudo singularity build {{image.sif}} {{recipe}}
```
{% endraw %}