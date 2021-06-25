---
layout: default
title: "jps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jps">
  <a href="/zh/common/jps.html">jps</a> <a href="#jps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示当前用户的 JVM 进程状态。
> 详细信息见：<https://docs.oracle.com/en/java/javase/11/tools/jps.html>.

#### 列出所有 JVM 进程：
```shell
jps
```
#### 列出所有 JVM 进程，只打印进程号：
```shell
jps -q
```
#### 显示传递给进程的参数：
```shell
jps -m
```
#### 显示所有进程的完整软件包名称：
```shell
jps -l
```
#### 显示传递给 JVM 的参数：
```shell
jps -v
```
{% endraw %}