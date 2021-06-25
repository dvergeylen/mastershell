---
layout: default
title: "ninja"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ninja">
  <a href="/en/common/ninja.html">ninja</a> <a href="#ninja"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Build system designed to be fast.
> More information: <https://ninja-build.org/manual.html>.

#### Build in the current directory:
```shell
ninja
```
#### Build a program in a given directory:
```shell
ninja -C {{path/to/directory}}
```
#### Show targets (e.g. `install` and `uninstall`):
```shell
ninja -t targets
```
#### Show help:
```shell
ninja -h
```
{% endraw %}