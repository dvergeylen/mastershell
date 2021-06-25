---
layout: default
title: "archlinux-java"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="archlinux-java">
  <a href="/zh/linux/archlinux-java.html">archlinux-java</a> <a href="#archlinux-java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 提供 Java 环境设置功能的一个帮助脚本。
> 更多信息：<https://github.com/michaellass/archlinux-java-run>.

#### 列出已安装的 Java 环境：
```shell
archlinux-java status
```
#### 设置默认的 Java 环境：
```shell
archlinux-java set {{java_environment}}
```
#### 取消默认的 Java 环境：
```shell
archlinux-java unset
```
#### 自动设置默认的 Java 环境：
```shell
archlinux-java fix
```
{% endraw %}