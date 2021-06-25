---
layout: default
title: "androguard"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="androguard">
  <a href="/zh/common/androguard.html">androguard</a> <a href="#androguard"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用python编写的一款针对安卓应用的逆向工程工具.
> 更多信息: <https://github.com/androguard/androguard>.

#### 展示Android manifest清单文件:
```shell
androguard axml {{路径/至/应用.apk}}
```
#### 展示app元数据 (版本和app ID):
```shell
androguard apkid {{路径/至/应用.apk}}
```
#### 反编译Java代码:
```shell
androguard decompile {{路径/至/应用.apk}} --output {{路径/至/目录}}
```
{% endraw %}