---
layout: default
title: "base32"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base32">
  <a href="/zh/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文件或标准输入编码到Base32或从Base32解码为标准输出。
> 更多信息： <https://www.gnu.org/software/coreutils/base32>.

#### 编码一个文件:
```shell
base32 {{文件名}}
```
#### 解码一个文件:
```shell
base32 --decode {{文件名}}
```
#### 从标准输入编码:
```shell
{{某指令}} | base32
```
#### 将标准输入解码:
```shell
{{某指令}} | base32 --decode
```
{% endraw %}