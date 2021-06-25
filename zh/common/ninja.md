---
layout: default
title: "ninja"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ninja">
  <a href="/zh/common/ninja.html">ninja</a> <a href="#ninja"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个快速的构建系统.
> 更多信息: <https://ninja-build.org/manual.html>.

#### 在当前目录下构建:
```shell
ninja
```
#### 在指定的目录中构建一个程序:
```shell
ninja -C {{路径}}
```
#### 查看 target（如 `install` 和 `uninstall`):
```shell
ninja -t targets
```
#### 查看帮助:
```shell
ninja -h
```
{% endraw %}