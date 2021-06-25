---
layout: default
title: "nautilus"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nautilus">
  <a href="/en/linux/nautilus.html">nautilus</a> <a href="#nautilus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Default file explorer for GNOME desktop environment.
> Also known as GNOME Files.
> More information: <https://manned.org/nautilus>.

#### Launch Nautilus:
```shell
nautilus
```
#### Launch Nautilus as root user:
```shell
sudo nautilus
```
#### Launch Nautilus and display a specific directory:
```shell
nautilus {{path/to/directory}}
```
#### Launch Nautilus with a specific file or directory selected:
```shell
nautilus --select {{path/to/file_or_directory}}
```
#### Launch Nautilus in a separated window:
```shell
nautilus --new-window
```
#### Close all Nautilus instances:
```shell
nautilus --quit
```
#### Display help:
```shell
nautilus --help
```
{% endraw %}