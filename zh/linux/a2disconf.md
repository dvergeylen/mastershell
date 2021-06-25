---
layout: default
title: "a2disconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2disconf">
  <a href="/zh/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上禁用 Apache 配置文件.
> 更多信息: <https://manpages.debian.org/latest/apache2/a2disconf.8.html>.

#### 禁用配置文件:
```shell
sudo a2disconf {{配置文件}}
```
#### 不显示信息性消息:
```shell
sudo a2disconf --quiet {{配置文件}}
```
{% endraw %}