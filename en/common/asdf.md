---
layout: default
title: "asdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asdf">
  <a href="/en/common/asdf.html">asdf</a> <a href="#asdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for managing versions of different packages.
> More information: <https://asdf-vm.com>.

#### List all available plugins:
```shell
asdf plugin-list-all
```
#### Install a plugin:
```shell
asdf plugin-add {{name}}
```
#### List all available versions for a package:
```shell
asdf list-all {{name}}
```
#### Install a specific version of a package:
```shell
asdf install {{name}} {{version}}
```
#### Set global version for a package:
```shell
asdf global {{name}} {{version}}
```
#### Set local version for a package:
```shell
asdf local {{name}} {{version}}
```
{% endraw %}