---
layout: default
title: "reg compare"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-compare">
  <a href="/zh/windows/reg-compare.html">reg compare</a> <a href="#reg-compare"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 比较注册表中的键和值.

#### 比较两个键中的所有值:
```shell
reg compare {{第一个键名}} {{第二个键名}}
```
#### 比较两个键中指定的值:
```shell
reg compare {{第一个键名}} {{第二个键名}} /v {{值}}
```
#### 比较两个键中的所有子键和值:
```shell
reg compare {{第一个键名}} {{第二个键名}} /s
```
#### 仅输出指定键之间匹配的结果:
```shell
reg compare {{第一个键名}} {{第二个键名}} /os
```
#### 输出两个键之间的匹配和差异:
```shell
reg compare {{第一个键名}} {{第二个键名}} /oa
```
{% endraw %}