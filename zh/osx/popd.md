---
layout: default
title: "popd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="popd">
  <a href="/zh/osx/popd.html">popd</a> <a href="#popd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过 pushd shell 内置程序删除目录堆栈中的目录.

#### 从堆栈中删除顶部目录，并用 `cd` 跳转到该目录:
```shell
popd
```
#### 删除第 n 个目录（从零开始，以用 `dirs` 打印的列表左侧开始）:
```shell
popd +N
```
#### 删除第 n 个目录（从零开始，以用 `dirs` 打印的列表右侧开始）:
```shell
popd -N
```
{% endraw %}