---
layout: default
title: "asciiart"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asciiart">
  <a href="/zh/linux/asciiart.html">asciiart</a> <a href="#asciiart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将图像转换为 ASCII.
> 更多信息: <https://github.com/nodanaonlyzuul/asciiart>.

#### 从文件中读取图像并以 ASCII 打印:
```shell
asciiart {{路径/image.jpg}}
```
#### 从 URL 中读取图像并以 ASCII 打印:
```shell
asciiart {{www.example.com/image.jpg}}
```
#### 选择输出宽度 (默认为 100):
```shell
asciiart -width {{50}} {{路径/image.jpg}}
```
#### 对 ASCII 输出进行着色:
```shell
asciiart --color {{路径/image.jpg}}
```
#### 选择输出格式 (默认格式为文本):
```shell
asciiart --format {{text|html}} {{路径/image.jpg}}
```
#### 反转字符映射:
```shell
asciiart --invert-chars {{路径/image.jpg}}
```
{% endraw %}