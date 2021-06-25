---
layout: default
title: "bashmarks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bashmarks">
  <a href="/zh/common/bashmarks.html">bashmarks</a> <a href="#bashmarks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用一个字母的命令，保存或者跳转到常用的目录
> 更多信息: <https://github.com/huyng/bashmarks>.

#### 可访问书签清单:
```shell
l
```
#### 保存当前目录到某书签里:
```shell
s {{书签名}}
```
#### 跳转到指定书签
```shell
g {{书签名}}
```
#### 打印书签目录内容
```shell
p {{书签名}}
```
#### 删除书签：
```shell
d {{书签名}}
```
{% endraw %}