---
layout: default
title: "systeminfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="systeminfo">
  <a href="/zh/windows/systeminfo.html">systeminfo</a> <a href="#systeminfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示本地或远程计算机的操作系统配置.

#### 显示本地计算机的操作系统配置:
```shell
systeminfo
```
#### 以指定的输出格式显示系统配置:
```shell
systeminfo /fo {{table|list|csv}}
```
#### 显示远程计算机的系统配置:
```shell
systeminfo /s {{远程主机名}} /u {{用户名}} /p {{密码}}
```
#### 显示详细的帮助信息:
```shell
systeminfo /?
```
{% endraw %}