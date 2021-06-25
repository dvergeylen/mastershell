---
layout: default
title: "conan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="conan">
  <a href="/en/common/conan.html">conan</a> <a href="#conan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The open source, decentralized and cross-platform package manager to create and share all your native binaries.
> More information: <https://conan.io/>.

#### Install packages based on `conanfile.txt`:
```shell
conan install {{.}}
```
#### Install packages and create configuration files for a specific generator:
```shell
conan install -g {{generator}}
```
#### Install packages, building from source:
```shell
conan install {{.}} --build
```
#### Search for locally installed packages:
```shell
conan search {{package}}
```
#### Search for remote packages:
```shell
conan search {{package}} -r {{remote}}
```
#### List remotes:
```shell
conan remote --list
```
{% endraw %}