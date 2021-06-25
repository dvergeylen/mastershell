---
layout: default
title: "choco new"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-new">
  <a href="/en/windows/choco-new.html">choco new</a> <a href="#choco-new"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate new package specification files with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-new>.

#### Create a new package skeleton:
```shell
choco new {{package_name}}
```
#### Create a new package with a specific version:
```shell
choco new {{package_name}} --version {{version}}
```
#### Create a new package with a specific maintainer name:
```shell
choco new {{package_name}} --maintainer {{maintainer_name}}
```
#### Create a new package in a custom output directory:
```shell
choco new {{package_name}} --output-directory {{path/to/directory}}
```
#### Create a new package with specific 32-bit and 64-bit installer URLs:
```shell
choco new {{package_name}} url="{{url}}" url64="{{url}}"
```
{% endraw %}