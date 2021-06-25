---
layout: default
title: "shasum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shasum">
  <a href="/zh/common/shasum.html">shasum</a> <a href="#shasum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 计算或检查加密 SHA 校验值.

#### 计算文件的 SHA1 校验值:
```shell
shasum {{文件名}}
```
#### 计算文件的 SHA256 校验值:
```shell
shasum --algorithm 256 {{文件名}}
```
#### 计算多个文件的 SHA512 校验值:
```shell
shasum --algorithm 512 {{文件名 1}} {{文件名 2}}
```
#### 计算一个文件内列出的所有的目录文件的相对应的总数:
```shell
shasum --check {{列表文件}}
```
#### 从标准输入中获取并计算 SHA1 校验值:
```shell
{{其他命令}} | shasum
```
{% endraw %}