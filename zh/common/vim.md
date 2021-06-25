---
layout: default
title: "vim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vim">
  <a href="/zh/common/vim.html">vim</a> <a href="#vim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vi IMproved, 一个程序员的文本编辑器，提供为不同类型的文档修改设计的多种模式
> 在`vim`内使用任何命令时请确认未使用中文输入法，否则可能会出现奇怪的问题
> 按下`i`来进入编辑模式，`<esc>`回到标准模式 （不允许普通的字符输入）
> 更多信息：<https://www.vim.org>.

#### 打开文档:
```shell
vim {{file}}
```
#### 进入编辑模式 （插入模式）:
```shell
<Esc>i
```
#### 复制 ("yank") 或剪切 ("delete") 当前行 （使用`P`来粘贴）:
```shell
<Esc>{{yy|dd}}
```
#### 撤销上一个操作:
```shell
<Esc>u
```
#### 在文件中搜寻 （按下 `n`/`N` 来在上一个 / 下一个结果中切换）:
```shell
<Esc>/{{search_pattern}}<Enter>
```
#### 对整个文件使用正则表达式进行替换:
```shell
<Esc>:%s/{{pattern}}/{{replacement}}/g<Enter>
```
#### 保存 （写入） 文件，然后退出:
```shell
<Esc>:wq<Enter>
```
#### 不保存退出:
```shell
<Esc>:q!<Enter>
```
{% endraw %}