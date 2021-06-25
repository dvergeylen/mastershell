---
layout: default
title: "logoff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logoff">
  <a href="/zh/windows/logoff.html">logoff</a> <a href="#logoff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 注销登录会话.

#### 注销当前会话:
```shell
logoff
```
#### 通过名称和 id 注销会话:
```shell
logoff {{会话名|会话 id}}
```
#### 在通过 RDP 连接的特定服务器上注销会话:
```shell
logoff {{会话名|会话 id}} /server:{{服务器名}}
```
{% endraw %}