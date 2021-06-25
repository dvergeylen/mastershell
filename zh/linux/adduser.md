---
layout: default
title: "adduser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adduser">
  <a href="/zh/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 添加用户的工具.
> 更多信息： <https://manpages.debian.org/latest/adduser/adduser.html>.

#### 创建一个新用户，在默认路径创建 home 目录，并提示用户设置密码:
```shell
adduser {{用户名}}
```
#### 创建一个新用户，不生成 home 目录:
```shell
adduser --no-create-home {{用户名}}
```
#### 创建一个新用户，并在指定路径下创建 home 目录:
```shell
adduser --home {{home 路径}} {{用户名}}
```
#### 创建一个新用户，并指定登录 shell:
```shell
adduser --shell {{shell 路径}} {{用户名}}
```
#### 创建一个新用户，并指定其用户组:
```shell
adduser --ingroup {{用户组}} {{用户名}}
```
{% endraw %}