---
layout: default
title: "konsole"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="konsole">
  <a href="/zh/linux/konsole.html">konsole</a> <a href="#konsole"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konsole: KDE 终端模拟器.
> 更多信息: <https://konsole.kde.org>.

#### 在特定目录中打开一个新的 Konsole:
```shell
konsole --workdir {{path/to/directory}}
```
#### 运行特定命令，退出窗口后不要关闭窗口:
```shell
konsole --noclose -e {{命令}}
```
#### 打开新标签页:
```shell
konsole --new-tab
```
#### 在后台打开 Konsole 并在按下 Ctrl+Shift+F12 (默认) 时显示在最前面:
```shell
konsole --background-mode
```
#### 使用紧急备冗配置文件打开 Konsole:
```shell
konsole --fallback-profile
```
{% endraw %}