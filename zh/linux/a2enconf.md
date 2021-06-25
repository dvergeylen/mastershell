---
layout: default
title: "a2enconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2enconf">
  <a href="/zh/linux/a2enconf.html">a2enconf</a> <a href="#a2enconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上启用 Apache 配置文件。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2enconf.8.html>.

#### 启用配置文件：
```shell
sudo a2enconf {{配置文件}}
```
#### 不显示信息性消息：
```shell
sudo a2enconf --quiet {{配置文件}}
```
{% endraw %}