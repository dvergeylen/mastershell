---
layout: default
title: "sfc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sfc">
  <a href="/zh/windows/sfc.html">sfc</a> <a href="#sfc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 扫描 Windows 系统文件的完整性.

#### 显示命令的使用方法:
```shell
sfc
```
#### 扫描所有的系统文件，如果可能的话，修复所有出现的问题:
```shell
sfc /scannow
```
#### 扫描系统文件，但不修复出现的问题:
```shell
sfc /verifyonly
```
#### 扫描指定的文件，如果可能的话，修复所有出现的问题:
```shell
sfc /scanfile={{文件的路径}}
```
#### 扫描指定的文件，但不修复出现的问题:
```shell
sfc /verifyfile={{文件的路径}}
```
#### 当离线修复时，指定引导目录:
```shell
sfc /offbootdir={{目录的路径}}
```
#### 当离线修复时，指定 Windows 目录:
```shell
sfc /offwindir={{文件的路径}}
```
{% endraw %}