---
layout: default
title: "arp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp">
  <a href="/zh/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示和操作系统的 ARP 缓存.
> 更多信息： <https://manned.org/arp>.

#### 显示当前的 ARP 表:
```shell
arp -a
```
#### 清除整个缓存:
```shell
sudo arp -a -d
```
#### 删除特定条目:
```shell
arp -d {{地址}}
```
#### 创建指定条目:
```shell
arp -s {{地址}} {{MAC 地址}}
```
{% endraw %}