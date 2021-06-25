---
layout: default
title: "apg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apg">
  <a href="/zh/common/apg.html">apg</a> <a href="#apg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 生成任意复杂度的随机密码.
> 更多信息： <https://manned.org/apg>.

#### 生成随机密码 （默认密码长度为 8 位）:
```shell
apg
```
#### 生成密码，包含至少 1 个符号 (S), 1 个数字 (N), 1 个大写字母 (C), 1 个小写字母 (L):
```shell
apg -M SNCL
```
#### 生成 16 个字符的密码:
```shell
apg -m {{16}}
```
#### 生成最大长度为 16 位的密码:
```shell
apg -x {{16}}
```
#### 生成未出现在字典中的密码（必须提供字典文件）
```shell
apg -r {{字典文件}}
```
{% endraw %}