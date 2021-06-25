---
layout: default
title: "addpart"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="addpart">
  <a href="/zh/linux/addpart.html">addpart</a> <a href="#addpart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将特定分区的存在告知 Linux 内核。
> 这个命令是 `add partition` ioctl 的简单封装。
> 更多信息：<https://manned.org/addpart>.

#### 将特定分区的存在告知 Linux 内核：
```shell
addpart {{设备名}} {{分区名}} {{起始点}} {{长度}}
```
{% endraw %}