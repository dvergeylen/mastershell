---
layout: default
title: "pathping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pathping">
  <a href="/zh/windows/pathping.html">pathping</a> <a href="#pathping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一种结合了`ping`和`tracert`功能的跟踪路由工具.

#### Ping 并追踪主机的路由:
```shell
pathping {{主机名}}
```
#### 不要对主机名执行 IP 地址的反向查找:
```shell
pathping {{主机名}} -n
```
#### 指定要搜索目标的最大跃点数（默认值为 30）:
```shell
pathping {{主机名}} -h {{最大跃点数}}
```
#### 指定 ping 之间等待的毫秒数（默认值为 240）:
```shell
pathping {{主机名}} -p {{时间}}
```
#### 指定每跳的查询数（默认值为 100）:
```shell
pathping {{主机名}} -q {{查询语句}}
```
#### 强制使用 IPV4:
```shell
pathping {{主机名}} -4
```
#### 强制使用 IPV6:
```shell
pathping {{主机名}} -6
```
#### 显示详细的使用帮助:
```shell
pathping /?
```
{% endraw %}