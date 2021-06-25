---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/zh/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印和拼接文件的工具.
> 更多信息： <https://www.gnu.org/software/coreutils/cat>.

#### 以标准输出，打印文件内容:
```shell
cat {{file}}
```
#### 多文件合并到目标文件:
```shell
cat {{file1}} {{file2}} > {{target_file}}
```
#### 多文件合并，并追加到目标文件:
```shell
cat {{file1}} {{file2}} >> {{target_file}}
```
#### 显示行号:
```shell
cat -n {{file}}
```
#### 显示不可打印和空白的字符 (使用`M-` 前缀标记非ASCII字符):
```shell
cat -v -t -e {{file}}
```
{% endraw %}