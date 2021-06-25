---
layout: default
title: "ark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ark">
  <a href="/zh/linux/ark.html">ark</a> <a href="#ark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE 归档工具。
> 更多信息： <https://docs.kde.org/stable5/en/kdeutils/ark/>.

#### 将存档解压缩到当前目录：
```shell
ark --batch {{存档名}}
```
#### 改变解压缩目录：
```shell
ark --batch --destination {{解压缩目录路径}} {{存档名}}
```
#### 创建一个原本不存在的存档并向它添加文件：
```shell
ark --add-to {{存档名}} {{文件1}} {{文件2}}
```
{% endraw %}