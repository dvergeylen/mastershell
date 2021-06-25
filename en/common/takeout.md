---
layout: default
title: "takeout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="takeout">
  <a href="/en/common/takeout.html">takeout</a> <a href="#takeout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Docker-based development-only dependency manager.
> More information: <https://github.com/tighten/takeout>.

#### Display a list of available services:
```shell
takeout enable
```
#### Enable a specific service:
```shell
takeout enable {{name}}
```
#### Enable a specific service with the default parameters:
```shell
takeout enable --default {{name}}
```
#### Display a list of enabled services:
```shell
takeout disable
```
#### Disable a specific service:
```shell
takeout disable {{name}}
```
#### Disable all services:
```shell
takeout disable --all
```
#### Start a specific container:
```shell
takeout start {{container_id}}
```
#### Stop a specific container:
```shell
takeout stop {{container_id}}
```
{% endraw %}