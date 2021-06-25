---
layout: default
title: "choco source"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-source">
  <a href="/en/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage sources for packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-source>.

#### List currently available sources:
```shell
choco source list
```
#### Add a new package source:
```shell
choco source add --name {{name}} --source {{url}}
```
#### Add a new package source with credentials:
```shell
choco source add --name {{name}} --source {{url}} --user {{username}} --password {{password}}
```
#### Add a new package source with a client certificate:
```shell
choco source add --name {{name}} --source {{url}} --cert {{path/to/certificate}}
```
#### Enable a package source:
```shell
choco source enable --name {{name}}
```
#### Disable a package source:
```shell
choco source disable --name {{name}}
```
#### Remove a package source:
```shell
choco source remove --name {{name}}
```
{% endraw %}