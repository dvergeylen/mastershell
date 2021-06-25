---
layout: default
title: "asar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asar">
  <a href="/zh/common/asar.html">asar</a> <a href="#asar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Electron 平台的文件打包工具.

#### 打包一个文件或目录:
```shell
asar pack {{文件或目录路径}} {{输出的 asar 文件}}
```
#### 解压一个 asar 文件:
```shell
asar extract {{asar 文件}}
```
#### 从 asar 文件中解压指定的文件:
```shell
asar extract-file {{asar 文件}} {{文件}}
```
#### 列出一个 asar 文件中的内容:
```shell
asar list {{asar 文件}}
```
{% endraw %}