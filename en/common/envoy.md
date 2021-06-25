---
layout: default
title: "envoy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="envoy">
  <a href="/en/common/envoy.html">envoy</a> <a href="#envoy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP-based task manager for Laravel remote servers.
> More information: <https://laravel.com/docs/envoy>.

#### Initialise a configuration file:
```shell
envoy init {{host_name}}
```
#### Run a task:
```shell
envoy run {{task_name}}
```
#### Run a task from a specific project:
```shell
envoy run --path {{path/to/directory}} {{task_name}}
```
#### Run a task and continue on failure:
```shell
envoy run --continue {{task_name}}
```
#### Dump a task as a bash script for inspection:
```shell
envoy run --pretend {{task_name}}
```
#### Connect to the specified server via SSH:
```shell
envoy ssh {{server_name}}
```
{% endraw %}