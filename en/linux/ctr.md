---
layout: default
title: "ctr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ctr">
  <a href="/en/linux/ctr.html">ctr</a> <a href="#ctr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage `containerd` containers and images.
> More information: <https://containerd.io>.

#### List all containers (running and stopped):
```shell
ctr containers list
```
#### List all images:
```shell
ctr images list
```
#### Pull an image:
```shell
ctr images pull {{image}}
```
#### Tag an image:
```shell
ctr images tag {{souce_image}}:{{source_tag}} {{target_image}}:{{target_tag}}
```
{% endraw %}