---
layout: default
title: "dmesg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmesg">
  <a href="/zh/sunos/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将内核消息写入标准输出.
> 更多信息： <https://www.unix.com/man-page/sunos/1m/dmesg>.

#### 显示内核消息:
```shell
dmesg
```
#### 显示此系统上可用的物理内存:
```shell
dmesg | grep -i memory
```
#### 一次显示一页内核消息:
```shell
dmesg | less
```
{% endraw %}