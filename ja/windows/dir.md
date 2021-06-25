---
layout: default
title: "dir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dir">
  <a href="/ja/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ディレクトリの内容を一覧表示します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### 現在のディレクトリの内容を表示します:
```shell
dir
```
#### 特定のディレクトリの内容を表示します:
```shell
dir {{ディレクトリパス}}
```
#### 非表示の内容を含む、現在のディレクトリの内容を表示します:
```shell
dir /A
```
#### 非表示の内容を含む、特定のディレクトリの内容を表示します:
```shell
dir {{ディレクトリパス}} /A
```
{% endraw %}