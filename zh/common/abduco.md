---
layout: default
title: "abduco"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="abduco">
  <a href="/zh/common/abduco.html">abduco</a> <a href="#abduco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 终端会话管理器.

#### 列出会话:
```shell
abduco
```
#### 附加到一个会话，如果不存在则新建它:
```shell
abduco -A {{会话名}} {{终端}}
```
#### 使用`dvtm`附加到一个会话，如果不存在则新建它:
```shell
abduco -A {{会话名}}
```
#### 从一个会话中分离:
```shell
Ctrl + \
```
#### 以只读模式附加到一个会话:
```shell
abduco -Ar {{会话名}}
```
{% endraw %}