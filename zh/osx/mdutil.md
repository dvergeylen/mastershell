---
layout: default
title: "mdutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdutil">
  <a href="/zh/osx/mdutil.html">mdutil</a> <a href="#mdutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 Spotlight（聚焦搜索） 用于搜索的索引数据.

#### 显示指定卷 ('/') 的索引状态:
```shell
mdutil -s {{/}}
```
#### 打开 / 关闭给定卷的 Spotlight 索引:
```shell
mdutil -i {{on|off}} {{指定卷文件夹}}
```
#### 清除索引数据并重新建立索引:
```shell
mdutil -E {{指定卷文件夹}}
```
{% endraw %}