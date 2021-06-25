---
layout: default
title: "zstd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zstd">
  <a href="/zh/common/zstd.html">zstd</a> <a href="#zstd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Zstandard 压缩来压缩 / 解压文件.
> 更多信息：<https://github.com/facebook/zstd>.

#### 将一个文件压缩到一个 `.zst` 后缀的压缩文件中:
```shell
zstd {{file}}
```
#### 解压缩一个文件:
```shell
zstd -d {{file}}.zst
```
#### 将文件解压缩到标准输出 (stdout):
```shell
zstd -dc {{file}}.zst
```
#### 使用指定的压缩等级来压缩一个文件.0 = 最差，19 = 最好 （默认等级是 3):
```shell
zstd -{{level}} {{file}}
```
#### 使用更多内存 （解压或压缩时） 来得到更高的压缩比:
```shell
zstd --ultra -{{level}} {{file}}
```
{% endraw %}