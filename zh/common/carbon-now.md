---
layout: default
title: "carbon-now"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="carbon-now">
  <a href="/zh/common/carbon-now.html">carbon-now</a> <a href="#carbon-now"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建漂亮的代码图片。
> 更多信息在 <https://github.com/mixn/carbon-now-cli>.

#### 使用默认设置从文件创建图片:
```shell
carbon-now {{文件}}
```
#### 使用默认设置从剪贴板创建图片:
```shell
carbon-now --from-clipboard
```
#### 使用默认设置从标准输入创建图片:
```shell
{{输入}} | carbon-now
```
#### 以交互方式创建图片以进行自定义设置，还可以选择保存预设:
```shell
carbon-now -i {{文件}}
```
#### 从先前保存的预设创建图片:
```shell
carbon-now -p {{预设}} {{文件}}
```
#### 从指定的文本行开始:
```shell
carbon-now -s {{行号}} {{文件}}
```
#### 结束于指定的文本行:
```shell
carbon-now -e {{行号}} {{文件}}
```
#### 在浏览器中打开图片而不是保存:
```shell
carbon-now --open {{文件}}
```
{% endraw %}