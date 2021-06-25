---
layout: default
title: "a2ensite"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2ensite">
  <a href="/zh/linux/a2ensite.html">a2ensite</a> <a href="#a2ensite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上启用 Apache 虚拟主机。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2ensite.8.html>.

#### 启用虚拟主机：
```shell
sudo a2ensite {{虚拟主机名}}
```
#### 不显示信息性消息：
```shell
sudo a2ensite --quiet {{虚拟主机名}}
```
{% endraw %}