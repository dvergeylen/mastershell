---
layout: default
title: "logcat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logcat">
  <a href="/zh/android/logcat.html">logcat</a> <a href="#logcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 转储系统消息日志。
> 更多信息见：https://developer.android.com/studio/command-line/logcat>.

#### 显示系统日志：
```shell
logcat
```
#### 将系统日志写入文件：
```shell
logcat -f {{文件路径}}
```
#### 显示与正则表达式匹配的行：
```shell
logcat --regex {{正则表达式}}
```
{% endraw %}