---
layout: default
title: "driverquery"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="driverquery">
  <a href="/zh/windows/driverquery.html">driverquery</a> <a href="#driverquery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示已安装设备驱动程序的信息.

#### 显示所有已安装设备驱动程序的列表:
```shell
driverquery
```
#### 以指定格式显示驱动程序的列表:
```shell
driverquery /fo {{table|list|csv}}
```
#### 显示带有列的驱动程序列表，以表明它们是否已签名:
```shell
driverquery /si
```
#### 排除输出列表中的标题:
```shell
driverquery /nh
```
#### 显示远程计算机的驱动程序列表:
```shell
driverquery /s {{主机名}} /u {{用户名}} /p {{密码}}
```
#### 显示详细信息的驱动程序列表
```shell
driverquery /v
```
#### 显示详细的使用信息:
```shell
driverquery /?
```
{% endraw %}