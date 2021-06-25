---
layout: default
title: "apache2ctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apache2ctl">
  <a href="/zh/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache HTTP web 服务器命令行管理工具。
> 基于 Debian 的操作系统自带该命令，基于 RHEL 的查看 `httpd`。

#### 启动 Apache 守护进程。如果已运行则发送一个消息：
```shell
sudo apache2ctl start
```
#### 关闭 Apache 守护进程：
```shell
sudo apache2ctl stop
```
#### 重启 Apache 守护进程：
```shell
sudo apache2ctl restart
```
#### 检查配置文件语法：
```shell
sudo apache2ctl -t
```
#### 列出已加载模块：
```shell
sudo apache2ctl -M
```
{% endraw %}