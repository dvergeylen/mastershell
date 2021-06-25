---
layout: default
title: "choco install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-install">
  <a href="/zh/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 下载一个或多个包.

#### 安装一个或多个用空格分隔的软件包:
```shell
choco install {{包名 包名 ..}}
```
#### 从一个自定义的配置文件中安装包:
```shell
choco install {{配置文件的路径}}
```
#### 安装一个特定的"nuspec"或"nupkg"文件:
```shell
choco install {{文件的路径}}
```
#### 安装一个指定版本的包:
```shell
choco install {{包名}} --version {{版本号}}
```
#### 允许安装一个包的多个版本:
```shell
choco install {{包名}} --allow-multiple
```
#### 自动确认所有提示:
```shell
choco install {{包名}} --yes
```
#### 从自定义的源处获取包:
```shell
choco install {{包名}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco install {{包名}} --user {{用户名}} --password {{密码}}
```
{% endraw %}