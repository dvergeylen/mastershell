---
layout: default
title: "fc-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fc-cache">
  <a href="/zh/linux/fc-cache.html">fc-cache</a> <a href="#fc-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 扫描字体目录，以便建立字体缓存文件。

#### 生成字体缓存文件：
```shell
fc-cache
```
#### 强制重建所有字体缓存文件，而不检查缓存是否为最新版本：
```shell
fc-cache -f
```
#### 删除字体缓存文件，然后生成新的字体缓存文件：
```shell
fc-cache -r
```
{% endraw %}