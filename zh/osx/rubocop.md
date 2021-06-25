---
layout: default
title: "rubocop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rubocop">
  <a href="/zh/osx/rubocop.html">rubocop</a> <a href="#rubocop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 格式化 Ruby 文件.

#### 检查当前目录中的所有文件（包括子目录）:
```shell
rubocop
```
#### 检查一个或多个指定文件或目录:
```shell
rubocop {{目录 / 文件名}} {{目录 /}}
```
#### 将输出写入指定文件:
```shell
rubocop --out {{目录 / 文件名}}
```
#### 查看规则列表（格式化规则）:
```shell
rubocop --show-cops
```
#### 排除格式规则:
```shell
rubocop --except {{规则 1}} {{规则 2}}
```
#### 只运行指定的规则:
```shell
rubocop --only {{规则 1}} {{规则 2}}
```
#### 自动更正文件（实验）:
```shell
rubocop --auto-correct
```
{% endraw %}