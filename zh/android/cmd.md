---
layout: default
title: "cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmd">
  <a href="/zh/android/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android 服务管理器。
> 更多信息见： <https://cs.android.com/android/platform/superproject/+/master:frameworks/native/cmds/cmd/>.

#### 列出所有正在运行的服务：
```shell
cmd -l
```
#### 调用指定服务：
```shell
cmd {{alarm}}
```
#### 调用服务同时传递参数：
```shell
cmd {{vibrator}} {{vibrate 300}}
```
{% endraw %}