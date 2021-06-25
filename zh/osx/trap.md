---
layout: default
title: "trap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="trap">
  <a href="/zh/osx/trap.html">trap</a> <a href="#trap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在进程或操作系统接收到信号后自动执行命令.
> 可用于对用户中断或其他操作执行清理.

#### 列出设置 trap 的可用信号:
```shell
trap -l
```
#### 列出当前 shell 程序的活动 trap 程序:
```shell
trap -p
```
#### 设置 trap 以在检测到一个或多个信号时执行命令:
```shell
trap 'echo "检测到信号 {{SIGHUP}}"' {{SIGHUP}}
```
#### 移除活动 trap:
```shell
trap - {{SIGHUP}} {{SIGINT}}
```
{% endraw %}