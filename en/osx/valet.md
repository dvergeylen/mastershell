---
layout: default
title: "valet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="valet">
  <a href="/en/osx/valet.html">valet</a> <a href="#valet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Laravel development environment that allows hosting sites via local tunnels on `http://<example>.test`.
> More information: <https://laravel.com/docs/8.x/valet>.

#### Start the valet daemon:
```shell
valet start
```
#### Register the current working directory as a path that Valet should search for sites:
```shell
valet park
```
#### View 'parked' paths:
```shell
valet paths
```
#### Serve a single site instead of an entire directory:
```shell
valet link app-name
```
#### Share a project via an Ngrok tunnel:
```shell
valet share
```
{% endraw %}