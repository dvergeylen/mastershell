---
layout: default
title: "choco info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-info">
  <a href="/zh/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有关 Chocolatey 包的详细信息.

#### 显示指定包的信息:
```shell
choco info {{包名}}
```
#### 显示一个本地已安装包的信息:
```shell
choco info {{包名}} --local-only
```
#### 从一个自定义的源来获取包的信息:
```shell
choco info {{包名}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco info {{包名}} --user {{用户名}} --password {{密码}}
```
{% endraw %}