---
layout: default
title: "bmaptool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bmaptool">
  <a href="/zh/common/bmaptool.html">bmaptool</a> <a href="#bmaptool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 便捷地创建或复制块文件映射（被设计的比`cp`或`dd`更快）.
> 更多信息: <https://source.tizen.org/documentation/reference/bmaptool>.

#### 使用图片生成块图文件:
```shell
bmaptool create -o {{blockmap格式文件.bmap}} {{图片文件}}
```
#### 复制图片到指定目录:
```shell
bmaptool copy --bmap {{blockmap格式文件}} {{图片文件}} {{/开发路径/sdb}}
```
#### 复制压缩后的图片到指定目录:
```shell
bmaptool copy --bmap {{blockmap格式文件}} {{图片文件.gz}} {{/开发路径/sdb}}
```
#### 复制图片的时候，不将图片转成块图:
```shell
bmaptool copy --nobmap {{图片文件}} {{/开发路径/sdb}}
```
{% endraw %}