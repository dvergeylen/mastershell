---
layout: default
title: "ping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ping">
  <a href="/zh/osx/ping.html">ping</a> <a href="#ping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向网络主机发送 ICMP 回显请求数据包.

#### Ping 指定的主机:
```shell
ping {{主机}}
```
#### 对主机执行指定定次数的 ping 操作:
```shell
ping -c {{次数}} {{主机}}
```
#### ping `主机` , 指定请求之间的间隔（以`秒`为单位）（默认为 1 秒）:
```shell
ping -i {{秒}} {{主机}}
```
#### Ping `主机`, 但不尝试查找地址的符号名:
```shell
ping -n {{主机}}
```
#### ping `主机` 并在收到数据包时响铃（如果您的终端支持）:
```shell
ping -a {{主机}}
```
#### ping `主机` 并打印接收数据包的时间（此选项是 Apple 的附加项）:
```shell
ping --apple-time {{主机}}
```
{% endraw %}