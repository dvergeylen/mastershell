---
layout: default
title: "flatpak"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flatpak">
  <a href="/en/linux/flatpak.html">flatpak</a> <a href="#flatpak"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build, install and run flatpak applications and runtimes.

#### Run an installed application:
```shell
flatpak run {{name}}
```
#### Install an application from a remote source:
```shell
flatpak install {{remote}} {{name}}
```
#### List all installed applications and runtimes:
```shell
flatpak list
```
#### Update all installed applications and runtimes:
```shell
flatpak update
```
#### Add a remote source:
```shell
flatpak remote-add --if-not-exists {{remote_name}} {{remote_url}}
```
#### List all configured remote sources:
```shell
flatpak remote-list
```
#### Remove an installed application:
```shell
flatpak remove {{name}}
```
#### Show information about an installed application:
```shell
flatpak info {{name}}
```
{% endraw %}