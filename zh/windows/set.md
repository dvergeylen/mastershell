---
layout: default
title: "set"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="set">
  <a href="/zh/windows/set.html">set</a> <a href="#set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或设置当前命令行实例的环境变量.

#### 列出当前所有环境变量:
```shell
set
```
#### 为一个环境变量设置指定的值:
```shell
set {{变量名}}={{值}}
```
#### 列出以指定字符串开头的环境变量:
```shell
set {{变量名}}
```
#### 提示用户输入指定变量的值:
```shell
set /p {{变量名}}={{提示信息}}
```
{% endraw %}