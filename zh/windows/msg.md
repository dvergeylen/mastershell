---
layout: default
title: "msg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="msg">
  <a href="/zh/windows/msg.html">msg</a> <a href="#msg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向指定的用户或会话发送信息.

#### 向指定的用户或会话发送信息:
```shell
msg {{用户名|会话名|会话 id}} {{信息}}
```
#### 从标准输入发送信息:
```shell
echo "{{信息}}" | msg {{用户名|会话名|会话 id}}
```
#### 向指定的服务器发送消息:
```shell
msg /server:{{服务器名称}} {{用户名|会话名|会话 id}}
```
#### 向当前计算机的所有用户发送消息:
```shell
msg *
```
#### 设置发送消息的延迟:
```shell
msg /time:{{秒}}
```
{% endraw %}