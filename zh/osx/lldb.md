---
layout: default
title: "lldb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lldb">
  <a href="/zh/osx/lldb.html">lldb</a> <a href="#lldb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> LLVM 低级调试器.

#### 调试可执行文件:
```shell
lldb {{可执行的命令}}
```
#### 将 `lldb` 附加到具有给定 PID 的正在运行的进程:
```shell
lldb -p {{进程号 PID}}
```
#### 等待使用给定名称的进程启动，然后附加到该进程上:
```shell
lldb -w -n {{进程名}}
```
{% endraw %}