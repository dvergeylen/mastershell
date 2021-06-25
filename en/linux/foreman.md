---
layout: default
title: "foreman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="foreman">
  <a href="/en/linux/foreman.html">foreman</a> <a href="#foreman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Procfile-based applications.

#### Start an application with the Procfile in the current directory:
```shell
foreman start
```
#### Start an application with a specified Procfile:
```shell
foreman start -f {{Procfile}}
```
#### Start a specific application:
```shell
foreman start {{process}}
```
#### Validate Procfile format:
```shell
foreman check
```
#### Run one-off commands with the process's environment:
```shell
foreman run {{command}}
```
#### Start all processes except the one named "worker":
```shell
foreman start -m all=1,{{worker}}=0
```
{% endraw %}