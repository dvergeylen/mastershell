---
layout: default
title: "dmesg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmesg">
  <a href="/zh/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或控制内核环形缓冲区。
> 更多信息：<https://manned.org/dmesg>.

#### 显示来自内核环形缓冲区的所有消息：
```shell
dmesg
```
#### 只显示严重错误级别的消息：
```shell
dmesg --level err
```
#### 等待新消息。仅在具有可读性的系统上支持此功能，类似于 `tail -f`（从内核 3.5.0 版本开始）：
```shell
dmesg -w
```
#### 显示此系统上有多少物理内存可用：
```shell
dmesg | grep -i memory
```
#### 以分页方式显示内核缓冲区的所有消息：
```shell
dmesg | less
```
#### 打印人类可读的时间戳（从内核 3.5.0 版本开始）：
```shell
dmesg -T
```
#### 启用人类可读的输出：
```shell
dmesg -H
```
#### 着色输出：
```shell
dmesg -L
```
{% endraw %}