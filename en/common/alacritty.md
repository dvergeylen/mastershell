---
layout: default
title: "alacritty"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alacritty">
  <a href="/en/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cross-platform, GPU-accelerated terminal emulator.
> More information: <https://github.com/alacritty/alacritty>.

#### Open a new Alacritty window:
```shell
alacritty
```
#### Run in a specific directory:
```shell
alacritty --working-directory {{path/to/directory}}
```
#### Run a command in a new Alacritty window:
```shell
alacritty -e {{command}}
```
#### Specify alternative configuration file (defaults to `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{path/to/config.yml}}
```
#### Run with live config reload enabled (can also be enabled by default in `alacritty.yml`):
```shell
alacritty --live-config-reload --config-file {{path/to/config.yml}}
```
{% endraw %}