---
layout: default
title: "apt-key"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-key">
  <a href="/zh/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian 和 Ubuntu 上的 APT 软件包管理器的密钥管理工具
> 更多信息： <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### 列出可信密钥:
```shell
apt-key list
```
#### 向可信密钥库中添加一个密钥:
```shell
apt-key add {{密钥文件.asc}}
```
#### 从可信密钥库中移除一个密钥:
```shell
apt-key del {{密钥 id}}
```
#### 向可信密钥库中添加一个远程密钥:
```shell
wget -qO - {{https://host.tld/filename.key}} | apt-key add -
```
#### 指定密钥 ID, 从密钥服务器中添加一个密钥:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{密钥 id}}
```
{% endraw %}