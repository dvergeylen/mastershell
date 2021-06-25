---
layout: default
title: "a2dismod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2dismod">
  <a href="/zh/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上禁用 Apache 模块。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2dismod.8.html>.

#### 禁用模块：
```shell
sudo a2dismod {{模块路径}}
```
#### 不显示信息性消息：
```shell
sudo a2dismod --quiet {{模块路径}}
```
{% endraw %}