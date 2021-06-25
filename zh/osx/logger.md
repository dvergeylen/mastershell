---
layout: default
title: "logger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logger">
  <a href="/zh/osx/logger.html">logger</a> <a href="#logger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向系统日志增加记录 (/var/log/syslog).

#### 向系统日志增加记录:
```shell
logger {{消息内容}}
```
#### 从 stdin 获取输入并记录到系统日志 syslog:
```shell
echo {{记录内容}} | logger
```
#### 将输出发送到在给定端口上运行的远程系统日志服务器。默认端口为 514:
```shell
echo {{记录内容}} | logger -h {{服务器名}} -P {{端口}}
```
#### 对记录的每一行使用特定的标签。默认值是登录用户的名:
```shell
echo {{记录内容}} | logger -t {{标签}}
```
#### 以给定的错误等级记录消息。默认是 `user.notice`. 使用 `man logger` 查询所有可选等级:
```shell
echo {{记录内容}} | logger -p {{user.warning}}
```
{% endraw %}