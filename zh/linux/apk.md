---
layout: default
title: "apk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apk">
  <a href="/zh/linux/apk.html">apk</a> <a href="#apk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alpine Linux 的包管理工具.

#### 从所有的远程仓库中更新仓库索引:
```shell
apk update
```
#### 安装一个新软件包:
```shell
apk add {{软件包}}
```
#### 移除一个软件包:
```shell
apk del {{软件包}}
```
#### 修复或更新软件包而不修改主依赖项:
```shell
apk fix {{软件包}}
```
#### 通过关键字查找软件包:
```shell
apk search {{关键字}}
```
#### 获取指定软件包的相关信息:
```shell
apk info {{软件包}}
```
{% endraw %}