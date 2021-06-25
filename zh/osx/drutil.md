---
layout: default
title: "drutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drutil">
  <a href="/zh/osx/drutil.html">drutil</a> <a href="#drutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 与 DVD 刻录机交互.

#### 从驱动器中弹出磁盘:
```shell
drutil eject
```
#### 将目录作为 iso9660 文件系统刻录到 DVD 上。完成后不验证和弹出:
```shell
drutil burn -noverify -eject -iso9660
```
{% endraw %}