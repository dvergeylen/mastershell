---
layout: default
title: "apport-bug"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apport-bug">
  <a href="/zh/linux/apport-bug.html">apport-bug</a> <a href="#apport-bug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 Ubuntu 上提交错误报告。
> 更多信息：<https://wiki.ubuntu.com/Apport>.

#### 报告整个系统的错误：
```shell
apport-bug
```
#### 报告某个软件包的错误：
```shell
apport-bug {{包名}}
```
#### 报告某个可执行文件的错误：
```shell
apport-bug {{可执行文件路径}}
```
#### 报告某个进程的错误：
```shell
apport-bug {{PID}}
```
{% endraw %}