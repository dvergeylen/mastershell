---
layout: default
title: "add-apt-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="add-apt-repository">
  <a href="/zh/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> apt 仓库管理。

#### 添加一个新的 apt 仓库：
```shell
add-apt-repository {{指定仓库}}
```
#### 移除一个 apt 仓库：
```shell
add-apt-repository --remove {{指定仓库}}
```
#### 添加一个仓库并更新缓存：
```shell
add-apt-repository --update {{指定仓库}}
```
#### 允许从指定仓库下载源码：
```shell
add-apt-repository --enable-source {{指定仓库}}
```
{% endraw %}