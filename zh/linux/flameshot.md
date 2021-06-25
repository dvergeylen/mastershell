---
layout: default
title: "flameshot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flameshot">
  <a href="/zh/linux/flameshot.html">flameshot</a> <a href="#flameshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 带有gui界面的Screenshot工具，支持基本的图像编辑，例如文本，形状，颜色和imgur.
> 更多信息: <https://flameshot.js.org>.

#### 在GUI模式下启动Flameshot:
```shell
flameshot launcher
```
#### 通过单击并拖动来截取屏幕截图:
```shell
flameshot gui
```
#### 全屏截图:
```shell
flameshot full
```
#### 将保存屏幕快照的路径设置为:
```shell
flameshot full --path {{path/to/directory}}
```
#### 将屏幕截图延迟N毫秒，然后输出到剪贴板:
```shell
flameshot full --delay {{2000}} --clipboard
```
{% endraw %}