---
layout: default
title: "finger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="finger">
  <a href="/zh/windows/finger.html">finger</a> <a href="#finger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 返回有关指定系统上的一个或多个用户的信息.
> 远程系统必须运行 Finger 服务.

#### 显示有关特定用户的信息:
```shell
finger {{用户名}}@{{主机名}}
```
#### 在指定的主机上显示所有用户的信息:
```shell
finger @{{主机名}}
```
#### 以更长的格式显示信息:
```shell
finger {{用户名}}@{{主机名}} -l
```
#### 显示帮助信息:
```shell
finger /?
```
{% endraw %}