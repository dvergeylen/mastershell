---
layout: default
title: "sips"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sips">
  <a href="/zh/osx/sips.html">sips</a> <a href="#sips"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 苹果的处理文件脚本系统.
> 光栅 / 查询图像 和 颜色同步 ICC 配置文件.

#### S 指定一个输出目录，这样原始文件就不会被修改:
```shell
sips --out {{目标 / 文件夹 / 输出文件夹}}
```
#### 以指定的大小对图像重新采样，图像纵横比可能会更改:
```shell
sips -z {{1920}} {{300}} {{图片文件。扩展名}}
```
#### 对图像重新取样，使高度和宽度不大于指定的大小（注意大写 Z）:
```shell
sips -Z {{1920}} {{300}} {{图片文件。扩展名}}
```
#### 对目录中的所有图像重新取样，以适应 960px 的宽度（保持纵横比）:
```shell
sips --resampleWidth {{960}} {{目标 / 文件夹 / 所有图片文件}}
```
#### 将图像从 CMYK 转换为 RGB:
```shell
sips --matchTo '/System/Library/ColorSync/Profiles/Generic RGB Profile.icc' {{目标 / 文件夹 / 图片。扩展}} {{目标 / 文件夹 / 输出文件夹}}
```
#### 从图像中删除 ColorSync ICC 配置:
```shell
sips -d profile --deleteColorManagementProperties {{目标 / 文件夹 / 图片。扩展}}
```
{% endraw %}