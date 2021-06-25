---
layout: default
title: "authconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="authconfig">
  <a href="/zh/linux/authconfig.html">authconfig</a> <a href="#authconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于设置系统认证资源的命令行界面。

#### 显示当前的配置（或空运行）：
```shell
authconfig --test
```
#### 设置服务器使用另一种不同的密码散列算法：
```shell
authconfig --update --passalgo={{算法名}}
```
#### 启用 LDAP 认证：
```shell
authconfig --update --enableldapauth
```
#### 关闭 LDAP 认证：
```shell
authconfig --update --disableldapauth
```
#### 开启网络信息服务（NIS）：
```shell
authconfig --update --enablenis
```
#### 开启 Kerberos：
```shell
authconfig --update --enablekrb5
```
#### 开启 Winbind （活动目录）认证：
```shell
authconfig --update --enablewinbindauth
```
#### 开启本地认证：
```shell
authconfig --update --enablelocauthorize
```
{% endraw %}