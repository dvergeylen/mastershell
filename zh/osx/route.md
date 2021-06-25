---
layout: default
title: "route"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="route">
  <a href="/zh/osx/route.html">route</a> <a href="#route"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 手动操作路由表.
> 需要 root 权限.

#### 通过网关向目标添加路由:
```shell
sudo route add {{路由 ip 地址}} {{网关地址}}
```
#### 通过网关向 子网 / 24 添加路由:
```shell
sudo route add {{子网 ip}}/24 {{网关地址}}
```
#### 在测试模式下运行（不做任何操作，只打印）:
```shell
sudo route -t add {{路由 ip 地址}}/24 {{网关地址}}
```
#### 删除所有路由:
```shell
sudo route flush
```
#### 删除特定路由:
```shell
sudo route delete {{路由 ip 地址}}/24
```
#### 查找并显示目标的路由（主机名或 IP 地址）:
```shell
sudo route get {{目标}}
```
{% endraw %}