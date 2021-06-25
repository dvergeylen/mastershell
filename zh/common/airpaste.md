---
layout: default
title: "airpaste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airpaste">
  <a href="/zh/common/airpaste.html">airpaste</a> <a href="#airpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在同一网络下共享信息和文件.
> 更多信息： <https://github.com/mafintosh/airpaste>.

#### 等待接收消息并显示接收到的信息:
```shell
airpaste
```
#### 发送文本:
```shell
echo {{文本}} | airpaste
```
#### 发送文件:
```shell
airpaste < {{文件的路径}}
```
#### 接收文件:
```shell
airpaste > {{文件的路径}}
```
#### 创建 / 加入频道:
```shell
airpaste {{频道名}}
```
{% endraw %}