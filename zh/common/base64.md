---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/zh/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文件或标准输入编码到Base64或从Base64解码为标准输出。
> 更多信息： <https://www.gnu.org/software/coreutils/base64>.

#### 编码一个文件:
```shell
base64 {{文件名}}
```
#### 解码一个文件:
```shell
base64 --decode {{文件名}}
```
#### 从标准输入编码:
```shell
{{某指令}} | base64
```
#### 将标准输入解码:
```shell
{{某指令}} | base64 --decode
```
{% endraw %}