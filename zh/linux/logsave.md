---
layout: default
title: "logsave"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logsave">
  <a href="/zh/linux/logsave.html">logsave</a> <a href="#logsave"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将一个命令的输出保存在日志文件中.
> 更多信息: <https://manned.org/logsave>.

#### 使用指定的参数执行命令并将其输出保存到日志文件中:
```shell
logsave {{path/to/logfile}} {{command}}
```
#### 从标准输入中获取输入并将其保存在日志文件中:
```shell
logsave {{logfile}} -
```
#### 将输出追加到日志文件，而不是替换其当前内容:
```shell
logsave -a {{logfile}} {{command}}
```
#### 显示详细输出:
```shell
logsave -v {{logfile}} {{command}}
```
{% endraw %}