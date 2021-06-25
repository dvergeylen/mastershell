---
layout: default
title: "wifi-password"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wifi-password">
  <a href="/zh/osx/wifi-password.html">wifi-password</a> <a href="#wifi-password"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 获取 wifi 的密码.
> 更多信息: <https://github.com/rauchg/wifi-password>.

#### 获取你当前登录的 wifi 的密码:
```shell
wifi-password
```
#### 获取特定 SSID 的 wifi 的密码:
```shell
wifi-password {{ssid}}
```
#### 仅输出密码:
```shell
wifi-password -q
```
{% endraw %}