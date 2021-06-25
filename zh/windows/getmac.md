---
layout: default
title: "getmac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getmac">
  <a href="/zh/windows/getmac.html">getmac</a> <a href="#getmac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示系统的 MAC 地址.

#### 显示当前系统的 MAC 地址:
```shell
getmac
```
#### 以特定格式显示详细信息:
```shell
getmac /fo {{table|list|csv}}
```
#### 排除输出列表中的标题:
```shell
getmac /nh
```
#### 显示一个远程主机的 MAC 地址:
```shell
getmac /s {{主机名}} /u {{用户名}} /p {{密码}}
```
#### 详细显示 MAC 地址信息:
```shell
getmac /v
```
#### 显示详细的帮助信息:
```shell
getmac /?
```
{% endraw %}