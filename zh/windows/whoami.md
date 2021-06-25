---
layout: default
title: "whoami"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whoami">
  <a href="/zh/windows/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有关当前用户的详细信息.

#### 显示当前用户的用户名:
```shell
whoami
```
#### 显示当前用户所属的组:
```shell
whoami /groups
```
#### 显示当前用户的权限:
```shell
whoami /priv
```
#### 显示当前用户的用户主体名称 (UPN):
```shell
whoami /upn
```
#### 显示当前用户的登录 id:
```shell
whoami /logonid
```
{% endraw %}