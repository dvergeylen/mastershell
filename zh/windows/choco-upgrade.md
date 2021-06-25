---
layout: default
title: "choco upgrade"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-upgrade">
  <a href="/zh/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 升级一个或多个包.

#### 升级一个或多个用空格分隔的软件包:
```shell
choco upgrade {{包名 包名 ..}}
```
#### 将一个包升级到指定版本:
```shell
choco upgrade {{包名}} --version {{版本号}}
```
#### 升级全部包:
```shell
choco upgrade all
```
#### 升级除指定的用逗号分隔的包之外的所有包:
```shell
choco upgrade all --except "{{包名 , 包名 ..}}"
```
#### 自动确认所有提示:
```shell
choco upgrade {{包名}} --yes
```
#### 从自定义源处升级包:
```shell
choco upgrade {{包名}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco upgrade {{包}} --user {{用户名}} --password {{密码}}
```
{% endraw %}