---
layout: default
title: "xctool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xctool">
  <a href="/zh/osx/xctool.html">xctool</a> <a href="#xctool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于构建 Xcode 项目的工具.

#### 在没有任何工作区的情况下生成单个项目:
```shell
xctool -project {{你的项目.名称}} -scheme {{方案}} build
```
#### 构建属于工作区的项目:
```shell
xctool -workspace {{你的工作区.名字}} -scheme {{方案}} build
```
#### 清理、构建和执行所有测试:
```shell
xctool -workspace {{你的工作区.名字}} -scheme {{方案}} clean build test
```
{% endraw %}