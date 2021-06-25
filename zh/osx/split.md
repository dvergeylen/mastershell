---
layout: default
title: "split"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="split">
  <a href="/zh/osx/split.html">split</a> <a href="#split"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 把一个文件拆分成几块.

#### 分割一个文件，每个分割部分有 10 行（除了最后一个）:
```shell
split -l {{10}} {{文件名}}
```
#### 用正则表达式拆分文件。匹配行将是下一个输出文件的第一行:
```shell
split -p {{cat|^[dh]og}} {{文件名}}
```
#### 拆分一个文件，每个拆分中有 512 个字节（除了最后一个文件，使用 512K 表示 Kb，512M 表示 Mb）:
```shell
split -b {{512}} {{文件名}}
```
{% endraw %}