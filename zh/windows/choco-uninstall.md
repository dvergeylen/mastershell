---
layout: default
title: "choco uninstall"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-uninstall">
  <a href="/zh/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 卸载一个或多个包.

#### 卸载一个或多个用空格分隔的软件包:
```shell
choco uninstall {{包名 『包名』 ..}}
```
#### 卸载一个指定版本的包:
```shell
choco uninstall {{包名}} --version {{版本号}}
```
#### 自动确认所有提示:
```shell
choco uninstall {{包名}} --yes
```
#### 卸载时同时删除其所有的依赖:
```shell
choco uninstall {{包名}} --remove-dependencies
```
#### 卸载全部包:
```shell
choco uninstall all
```
{% endraw %}