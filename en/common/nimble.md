---
layout: default
title: "nimble"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nimble">
  <a href="/en/common/nimble.html">nimble</a> <a href="#nimble"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package manager for the Nim programming language.
> Manage Nim projects and their dependencies.
> More information: <https://github.com/nim-lang/nimble>.

#### Search for packages:
```shell
nimble search {{search_string}}
```
#### Install a package:
```shell
nimble install {{package_name}}
```
#### List installed packages:
```shell
nimble list -i
```
#### Create a new Nimble package in the current directory:
```shell
nimble init
```
#### Build a Nimble package:
```shell
nimble build
```
#### Install a Nimble package:
```shell
nimble install
```
{% endraw %}