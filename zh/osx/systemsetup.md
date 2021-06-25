---
layout: default
title: "systemsetup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="systemsetup">
  <a href="/zh/osx/systemsetup.html">systemsetup</a> <a href="#systemsetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 配置系统首选项计算机设置.

#### 启用远程登录 (SSH):
```shell
systemsetup -setremotelogin on
```
#### 指定时区、NTP 服务器并启用网络时间:
```shell
systemsetup -settimezone {{美国 / 太平洋}} -setnetworktimeserver {{us.pool.ntp.org}} -setusingnetworktime on
```
#### 使机器从不休眠，并在电源故障或内核死机时自动重新启动:
```shell
systemsetup -setsleep off -setrestartpowerfailure on -setrestartfreeze on
```
#### disks 选择启动:
```shell
systemsetup -liststartupdisks
```
#### 指定新的启动盘:
```shell
systemsetup -setstartupdisk {{路径}}
```
{% endraw %}