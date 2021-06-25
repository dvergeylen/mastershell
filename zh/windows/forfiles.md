---
layout: default
title: "forfiles"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="forfiles">
  <a href="/zh/windows/forfiles.html">forfiles</a> <a href="#forfiles"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 选择一个或多个文件以执行指定的命令.

#### 在当前的目录中寻找文件:
```shell
forfiles
```
#### 在一个指定目录中寻找文件:
```shell
forfiles /p {{目录的路径}}
```
#### 为每个文件执行指定的命令:
```shell
forfiles /c "{{命令}}"
```
#### 使用通配符来寻找指定的文件:
```shell
forfiles /m {{通配符}}
```
#### 递归寻找文件:
```shell
forfiles /s
```
#### 搜索超过 5 天的文件:
```shell
forfiles /d {{+5}}
```
{% endraw %}