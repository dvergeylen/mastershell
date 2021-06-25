---
layout: default
title: "apt-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-file">
  <a href="/zh/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 apt 软件包中查找文件，其中也包括未安装的软件
> 更多信息： <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### 更新元数据的数据库:
```shell
sudo apt update
```
#### 查找包含指定文件或路径的软件包:
```shell
apt-file search {{文件名或路径}}
```
#### 列出指定包的内容:
```shell
apt-file list {{软件包名}}
```
{% endraw %}