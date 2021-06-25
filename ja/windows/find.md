---
layout: default
title: "find"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="find">
  <a href="/ja/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 1つ以上のファイルで指定された文字列を検索します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### 指定された文字列を含む行を検索します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}}
```
#### 指定された文字列を含まない行を表示します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}} /v
```
#### 指定された文字列を含む行数を表示します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}} /c
```
#### 行リストとともに行番号を表示します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}} /n
```
{% endraw %}