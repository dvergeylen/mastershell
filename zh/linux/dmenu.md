---
layout: default
title: "dmenu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmenu">
  <a href="/zh/linux/dmenu.html">dmenu</a> <a href="#dmenu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 动态菜单。
> 根据文本输入创建菜单，其中每一项都在新行中。

#### 显示 `ls` 命令输出的菜单：
```shell
{{ls}} | dmenu
```
#### 显示包含自定义项目的菜单，并用新行（`\n`）分隔：
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu
```
#### 让用户在多个项目之间进行选择，然后将所选项目保存到文件中：
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu > {{color.txt}}
```
#### 在特定的监视器上启动 `dmenu`：
```shell
ls | dmenu -m {{1}}
```
#### 在屏幕底部显示 `dmenu`：
```shell
ls | dmenu -b
```
{% endraw %}