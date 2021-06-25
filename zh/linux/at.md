---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/zh/linux/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在指定时间执行命令.
> 更多信息： <https://man.archlinux.org/man/at.1>.

#### 打开`at`提示符创建一组新的定时命令，按`Ctrl + D`保存并退出:
```shell
at {{hh:mm:ss}}
```
#### 运行命令并通过本地电子邮件程序（例如 sendmail) 发送运行结果:
```shell
at {{hh:mm:ss}} -m
```
#### 在指定时间执行一个脚本:
```shell
at {{hh:mm:ss}} -f {{文件路径}}
```
{% endraw %}