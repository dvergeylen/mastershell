---
layout: default
title: "wapm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wapm">
  <a href="/en/common/wapm.html">wapm</a> <a href="#wapm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The WebAssembly package manager.
> More information: <https://wapm.io/help/reference>.

#### Interactively create a new `wapm.toml` file:
```shell
wapm init
```
#### Download all the packages listed as dependencies in `wapm.toml`:
```shell
wapm install
```
#### Download a specific version of a package and add it to the list of dependencies in wapm.toml:
```shell
wapm install {{package_name}}@{{version}}
```
#### Download a package and install it globally:
```shell
wapm install --global {{package_name}}
```
#### Uninstall a package and remove it from the list of dependencies in `wapm.toml`:
```shell
wapm uninstall {{package_name}}
```
#### Print a tree of locally-installed dependencies:
```shell
wapm list
```
#### List top-level globally installed packages:
```shell
wapm list --global
```
#### Execute a package command using the Wasmer runtime:
```shell
wapm run {{command_name}} {{arguments}}
```
{% endraw %}