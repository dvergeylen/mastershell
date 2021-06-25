---
layout: default
title: "choco search"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-search">
  <a href="/zh/windows/choco-search.html">choco search</a> <a href="#choco-search"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 搜索一个本地或远程的包.

#### 搜索一个包:
```shell
choco search {{查询语句}}
```
#### 搜索一个本地的包:
```shell
choco search {{查询语句}} --local-only
```
#### 只显示包含完全匹配的结果:
```shell
choco search {{查询语句}} --exact
```
#### 自动确认所有提示:
```shell
choco search {{查询语句}} --yes
```
#### 从自定义的源处搜索包:
```shell
choco search {{查询语句}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco search {{查询语句}} --user {{用户名}} --password {{密码}}
```
{% endraw %}