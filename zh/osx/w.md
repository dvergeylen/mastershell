---
layout: default
title: "w"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="w">
  <a href="/zh/osx/w.html">w</a> <a href="#w"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示谁登录以及他们在做什么.
> 打印用户登录、tty、远程主机、登录时间、空闲时间、当前进程.

#### 显示登录用户信息:
```shell
w
```
#### 显示没有标题的登录用户信息:
```shell
w -h
```
#### 显示有关已登录用户的信息，按其空闲时间排序:
```shell
w -i
```
{% endraw %}