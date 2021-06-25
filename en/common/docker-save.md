---
layout: default
title: "docker save"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-save">
  <a href="/en/common/docker-save.html">docker save</a> <a href="#docker-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Export one or more docker images to archive.
> More information: <https://docs.docker.com/engine/reference/commandline/save/>.

#### Save an image by redirecting stdout to a tar archive:
```shell
docker save {{image}}:{{tag}} > {{path/to/file.tar}}
```
#### Save an image to a tar archive:
```shell
docker save --output {{path/to/file.tar}} {{image}}:{{tag}}
```
#### Save all tags of the image:
```shell
docker save --output {{path/to/file.tar}} {{image_name}}
```
#### Cherry-pick particular tags of an image to save:
```shell
docker save --output {{path/to/file.tar}} {{image_name:tag1 image_name:tag2 ...}}
```
{% endraw %}