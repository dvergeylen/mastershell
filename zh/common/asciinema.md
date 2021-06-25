---
layout: default
title: "asciinema"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asciinema">
  <a href="/zh/common/asciinema.html">asciinema</a> <a href="#asciinema"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 录制和播放终端会话，也可以把他们分享到 asciinema.org.

#### 将本地安装的`asciinema`与 asciinema.org 账号关联:
```shell
asciinema auth
```
#### 进行新的录制（完成后，将提示用户上传或在本地保存:
```shell
asciinema rec
```
#### 进行新的录制，保存到本地的文件中:
```shell
asciinema rec {{文件路径}}.cast
```
#### 从本地文件中播放终端录屏:
```shell
asciinema play {{文件路径}}.cast
```
#### 在 asciinema.org 中播放终端录屏:
```shell
asciinema play https://asciinema.org/a/{{文件 ID}}
```
#### 进行新的录制，将闲置时间设置为最多 2.5 秒:
```shell
asciinema rec -i {{2.5}}
```
#### 打印本地保存的录像的完整输出:
```shell
asciinema cat {{文件路径}}.cast
```
#### 从本地上传一个录屏到 asciinema.org:
```shell
asciinema upload {{文件路径}}.cast
```
{% endraw %}