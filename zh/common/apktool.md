---
layout: default
title: "apktool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apktool">
  <a href="/zh/common/apktool.html">apktool</a> <a href="#apktool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> APK文件反编译工具
> 更多信息: <https://ibotpeaches.github.io/Apktool/>.

#### 反编译:
```shell
apktool d {{应用.apk}}
```
#### 将一个文件夹打包为apk文件:
```shell
apktool b {{路径/到/目录}}
```
#### 安装并存储框架:
```shell
apktool if {{框架.apk}}
```
{% endraw %}