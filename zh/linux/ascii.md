---
layout: default
title: "ascii"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ascii">
  <a href="/zh/linux/ascii.html">ascii</a> <a href="#ascii"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示 ASCII 字符的别名。
> 更多信息：<http://www.catb.org/~esr/ascii/>.

#### 显示一个 ASCII 字符的别名：
```shell
ascii {{a}}
```
#### 以较短和脚本友好模式显示 ASCII 字符的别名：
```shell
ascii -t {{a}}
```
#### 显示多个 ASCII 字符的别名：
```shell
ascii -s {{tldr}}
```
#### 显示十进制 ASCII 字符表：
```shell
ascii -d
```
#### 显示十六进制 ASCII 字符表：
```shell
ascii -x
```
#### 显示八进制 ASCII 字符表：
```shell
ascii -o
```
#### 显示二进制 ASCII 字符表：
```shell
ascii -b
```
#### 显示选项总结和整个 ASCII 字符表：
```shell
ascii
```
{% endraw %}