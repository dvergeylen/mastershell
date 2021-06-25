---
layout: default
title: "sysctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sysctl">
  <a href="/zh/osx/sysctl.html">sysctl</a> <a href="#sysctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 访问内核状态信息.

#### 显示所有可用变量及其值:
```shell
sysctl -a
```
#### 显示 Apple 型号标识符:
```shell
sysctl -n hw.model
```
#### 显示 CPU 模型:
```shell
sysctl -n machdep.cpu.brand_string
```
#### 显示可用的 CPU 功能 (MMX, SSE, SSE2, SSE3, AES, 等）:
```shell
sysctl -n machdep.cpu.features
```
#### 设置一个可更改的内核状态变量:
```shell
sysctl -w {{部分。可修改的变量}}={{值}}
```
{% endraw %}