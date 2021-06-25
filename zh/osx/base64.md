---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/zh/osx/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Base64 来进行编码和解码.

#### 编码目标文件:
```shell
base64 --input={{目标文件}}
```
#### 解码目标文件:
```shell
base64 --decode --input={{base64 编码文件}}
```
#### 通过标准输入管道进行解码:
```shell
echo -n {{目标字符串}} | base64
```
#### 解码标准输入管道内容:
```shell
echo -n {{base64 字符串}} | base64 --decode
```
{% endraw %}