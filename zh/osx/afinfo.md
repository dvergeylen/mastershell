---
layout: default
title: "afinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="afinfo">
  <a href="/zh/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示音频文件元数据 (Metadata) 详细信息 (OS X).
> OS X 自带命令.

#### 显示给定音频文件的详细信息:
```shell
afinfo {{目标 / 路径 / 文件}}
```
#### 显示简化的音频文件信息 (单行):
```shell
afinfo -b {{目标 / 路径 / 文件}}
```
#### 显示音频文件的元数据信息以及其 InfoDictionary 词典:
```shell
afinfo -i {{目标 / 路径 / 文件}}
```
#### 以 xml 格式显示音频文件信息:
```shell
afinfo -x {{目标 / 路径 / 文件}}
```
#### 显示警告信息 (如存在):
```shell
afinfo --warnings {{目标 / 路径 / 文件}}
```
#### 显示完整用法帮助:
```shell
afinfo -h
```
{% endraw %}