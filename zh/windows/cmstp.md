---
layout: default
title: "cmstp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmstp">
  <a href="/zh/windows/cmstp.html">cmstp</a> <a href="#cmstp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于管理连接服务配置文件的命令行工具.

#### 安装指定的配置文件:
```shell
cmstp "{{配置文件的路径}}"
```
#### 安装时不创建桌面快捷方式:
```shell
cmstp /ns "{{配置文件的路径}}"
```
#### 安装时不检查依赖:
```shell
cmstp /nf "{{配置文件的路径}}"
```
#### 仅为当前用户安装:
```shell
cmstp /su "{{配置文件的路径}}"
```
#### 为所有用户安装 （需要管理员权限）:
```shell
cmstp /au "{{配置文件的路径}}"
```
#### 静默安装:
```shell
cmstp /s "{{配置文件的路径}}"
```
#### 卸载一个指定的配置文件:
```shell
cmstp /u "{{配置文件的路径}}"
```
#### 静默删除:
```shell
cmstp /u /s "{{配置文件的路径}}"
```
{% endraw %}