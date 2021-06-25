---
layout: default
title: "apt-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-cache">
  <a href="/zh/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian 和 Ubuntu 的包查询工具.
> 更多信息： <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### 在当前的软件源中查找一个软件包:
```shell
apt-cache search {{软件包}}
```
#### 显示指定软件包的相关信息:
```shell
apt-cache show {{软件包}}
```
#### 查看一个软件包是否安装或是否为最新:
```shell
apt-cache policy {{软件包}}
```
#### 显示一个软件包的依赖项:
```shell
apt-cache depends {{软件包}}
```
#### 列出依赖指定软件包的所有软件包:
```shell
apt-cache rdepends {{软件包}}
```
{% endraw %}