---
layout: default
title: "choco list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-list">
  <a href="/zh/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 显示包列表.

#### 列出所有可用的包:
```shell
choco list
```
#### 列出所有本地已安装的包:
```shell
choco list --local-only
```
#### 显示包含本地程序的列表:
```shell
choco list --include-programs
```
#### 只显示已批准的包:
```shell
choco list --approved-only
```
#### Specify a custom source to display packages from 指定一个源来显示包列表:
```shell
choco list --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco list --user {{用户名}} --password {{密码}}
```
{% endraw %}