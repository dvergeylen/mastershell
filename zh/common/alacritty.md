---
layout: default
title: "alacritty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alacritty">
  <a href="/zh/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 跨平台，GPU 加速的终端模拟器.
> 更多信息： <https://github.com/alacritty/alacritty>.

#### 打开一个新的 Alacritty 窗口:
```shell
alacritty
```
#### 运行在指定目录中：
```shell
alacritty --working-directory {{路径}}
```
#### 在新的 Alacritty 窗口中运行命令:
```shell
alacritty -e {{命令}}
```
#### 指定备用配置文件 (默认在 `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{路径/config.yml}}
```
#### 在启用实时配置重新加载的情况下运行（默认情况下也可以在 `alacritty.yml` 中启用）:
```shell
alacritty --live-config-reload --config-file {{路径/config.yml}}
```
{% endraw %}