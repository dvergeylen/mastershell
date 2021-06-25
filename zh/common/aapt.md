---
layout: default
title: "aapt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aapt">
  <a href="/zh/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 安卓资源包工具（Android Asset Packaging Tools）.
> 该工具可以查看，创建， 更新资源压缩包(zip, jar, apk)。

#### 列出资源压缩包里的内容:
```shell
aapt list {{路径/到/应用.apk}}
```
#### 查看APK包内指定的内容 (版本, 权限许可等):
```shell
aapt dump badging {{路径/到/应用.apk}}
```
#### 打包生成资源压缩包:
```shell
aapt package -F {{路径/到/应用.apk}} {{路径/到/目录}}
```
{% endraw %}