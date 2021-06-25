---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/zh/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可以打印并且合并文件的命令.
> `cat`的复制品，外加无法高亮和git集成.
> 更多信息: <https://github.com/sharkdp/bat>.

#### 文件内容打印:
```shell
bat {{文件}}
```
#### 多文件合并到目标文件:
```shell
bat {{文件1}} {{文件2}} > {{目标文件}}
```
#### 在指定文件后追加多个文件合并的内容:
```shell
bat {{文件1}} {{文件2}} >> {{目标文件}}
```
#### 打印时，显示行号:
```shell
bat -n {{文件}}
```
#### 高亮一个json文件:
```shell
bat --language json {{文件.json}}
```
#### 受支持的语言清单:
```shell
bat --list-languages
```
{% endraw %}