---
layout: default
title: "a2dissite"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2dissite">
  <a href="/zh/linux/a2dissite.html">a2dissite</a> <a href="#a2dissite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上禁用 Apache 虚拟主机。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2dissite.8.html>.

#### 禁用虚拟主机：
```shell
sudo a2dissite {{虚拟主机名}}
```
#### 不显示信息性消息：
```shell
sudo a2dissite --quiet {{虚拟主机名}}
```
{% endraw %}