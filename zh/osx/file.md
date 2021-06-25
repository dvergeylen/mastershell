---
layout: default
title: "file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="file">
  <a href="/zh/osx/file.html">file</a> <a href="#file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 确定文件类型.

#### 提供指定文件类型的描述，对于没有文件扩展名的文件可以正常工作:
```shell
file {{文件名}}
```
#### 查看压缩文件并确定其中的文件类型:
```shell
file -z {{xxx.zip}}
```
#### 允许文件与特殊文件或设备文件一起使用:
```shell
file -s {{文件名}}
```
#### 不要在第一个文件类型匹配时停止；继续执行直到文件结束:
```shell
file -k {{文件名}}
```
#### 确定文件的 mime 编码类型:
```shell
file -I {{文件名}}
```
{% endraw %}