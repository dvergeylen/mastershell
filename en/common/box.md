---
layout: default
title: "box"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="box">
  <a href="/en/common/box.html">box</a> <a href="#box"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP application for building and managing Phars.
> More information: <https://github.com/box-project/box>.

#### Compile a new Phar file:
```shell
box compile
```
#### Compile a new Phar file using a specific config file:
```shell
box compile -c {{path/to/config}}
```
#### Display information about the PHAR PHP extension:
```shell
box info
```
#### Display information about a specific Phar file:
```shell
box info {{path/to/phar_file}}
```
#### Validate the first found config file in the working directory:
```shell
box validate
```
#### Verify the signature of a specific Phar file:
```shell
box verify {{path/to/phar_file}}
```
#### Display all available commands and options:
```shell
box help
```
{% endraw %}