---
layout: default
title: "virtualboxvm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virtualboxvm">
  <a href="/en/windows/virtualboxvm.html">virtualboxvm</a> <a href="#virtualboxvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The VirtualBox virtual machine management CLI.
> More information: <https://www.virtualbox.org>.

#### Start a virtual machine:
```shell
virtualboxvm --startvm {{name|uuid}}
```
#### Start a virtual machine in fullscreen mode:
```shell
virtualboxvm --startvm {{name|uuid}} --fullscreen
```
#### Mount the specified DVD image file:
```shell
virtualboxvm --startvm {{name|uuid}} --dvd {{path/to/image_file}}
```
#### Display a command-line window with debug information:
```shell
virtualboxvm --startvm {{name|uuid}} --debug-command-line
```
#### Start a virtual machine in a paused state:
```shell
virtualboxvm --startvm {{name|uuid}} --start-paused
```
{% endraw %}