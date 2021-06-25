---
layout: default
title: "rdpsign"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rdpsign">
  <a href="/zh/windows/rdpsign.html">rdpsign</a> <a href="#rdpsign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于签名远程桌面协议（RDP）文件的工具.

#### 为一个 RDP 文件签名:
```shell
rdpsign {{文件路径.rdp}}
```
#### 使用一个指定的 sha256 哈希值为 RDP 文件签名:
```shell
rdpsign {{文件路径.rdp}} /sha265 {{哈希值}}
```
#### 启用静默输出:
```shell
rdpsign {{文件路径.rdp}} /q
```
#### 显示详细的信息、警告和状态:
```shell
rdpsign {{文件路径.rdp}} /v
```
#### 在不更新文件的情况下将输出显示到标准输出来测试签名:
```shell
rdpsign {{文件路径.rdp}} /l
```
{% endraw %}