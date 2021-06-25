---
layout: default
title: "export"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="export">
  <a href="/zh/osx/export.html">export</a> <a href="#export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 命令为当前 shell 中的子进程进行环境变量设置.

#### 设置为新的环境变量:
```shell
export {{某变量名}}={{值}}
```
#### 删除环境变量:
```shell
export -n {{某变量名}}
```
#### 给 PATH 追加新的路径进去:
```shell
export PATH=$PATH:{{追加的 path 路径}}
```
{% endraw %}