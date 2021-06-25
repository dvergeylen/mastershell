---
layout: default
title: "a2enmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2enmod">
  <a href="/zh/linux/a2enmod.html">a2enmod</a> <a href="#a2enmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上启用 Apache 模块。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2enmod.8.html>.

#### 启用模块：
```shell
sudo a2enmod {{模块名}}
```
#### 不显示信息性消息：
```shell
sudo a2enmod --quiet {{模块名}}
```
{% endraw %}