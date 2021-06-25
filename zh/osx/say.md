---
layout: default
title: "say"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="say">
  <a href="/zh/osx/say.html">say</a> <a href="#say"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文本转换为语音.

#### 大声说出一个句子:
```shell
say "{{你好，世界！}}"
```
#### 播放文本文件内容音频:
```shell
say -f {{文件名.txt}}
```
#### 用自定义的语音和语音速率说出一个句子:
```shell
say -v {{语音库名}} -r {{每分钟多少词}} "{{你好，我可以说中文.}}"
```
#### 列出可用的语音库:
```shell
say --voice="?"
```
#### 创建文本的音频文件:
```shell
say -o {{文件名.aiff}} "{{你好，请将录音内容输出到文件.}}"
```
{% endraw %}