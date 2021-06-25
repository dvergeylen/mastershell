---
layout: default
title: "oathtool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="oathtool">
  <a href="/zh/osx/oathtool.html">oathtool</a> <a href="#oathtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OATH 一次性密码工具.

#### 生成 TOTP 令牌（行为类似于 Google Authenticator）:
```shell
oathtool --totp --base32 {{密码}}
```
#### 根据给定时间产生特定的 TOTP 令牌:
```shell
oathtool --totp --now {{2004-02-29 16:21:42}} --base32 {{密码}}
```
#### 验证 TOTP 令牌:
```shell
oathtool --totp --base32 {{密码}} {{令牌}}
```
{% endraw %}