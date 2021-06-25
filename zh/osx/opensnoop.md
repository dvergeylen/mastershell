---
layout: default
title: "opensnoop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="opensnoop">
  <a href="/zh/osx/opensnoop.html">opensnoop</a> <a href="#opensnoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 跟踪系统中打开的文件标识符.

#### 输出当前系统内被打开的所有文件:
```shell
sudo opensnoop
```
#### 跟踪给定进程名，打开的所有文件:
```shell
sudo opensnoop -n {{进程名}}
```
#### 跟踪给定 PID（进程号）, 打开的所有文件:
```shell
sudo opensnoop -p {{PID 进程号}}
```
#### 跟踪打开了指定文件的继承:
```shell
sudo opensnoop -f {{路径 / 文件}}
```
{% endraw %}