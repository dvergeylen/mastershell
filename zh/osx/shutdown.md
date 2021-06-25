---
layout: default
title: "shutdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shutdown">
  <a href="/zh/osx/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 关闭并重新启动系统.

#### 立即关机:
```shell
shutdown -h now
```
#### 立即休眠:
```shell
shutdown -s now
```
#### 立即重启:
```shell
shutdown -r now
```
#### 倒计时 5 分钟重启:
```shell
shutdown -r +{{5}}
```
{% endraw %}