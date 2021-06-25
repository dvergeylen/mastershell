---
layout: default
title: "attrib"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="attrib">
  <a href="/ja/windows/attrib.html">attrib</a> <a href="#attrib"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ファイルまたはディレクトリの属性を表示または変更します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/attrib>.

#### 現在のディレクトリ内のファイルの属性を表示します:
```shell
attrib
```
#### 現在のディレクトリとサブディレクトリにあるファイルの属性を表示します:
```shell
attrib /S
```
#### 現在のディレクトリとサブディレクトリ内のファイルとディレクトリの属性を表示します:
```shell
attrib /S /D
```
#### ファイルに読み取り専用属性を追加します:
```shell
attrib +R {{ファイル名.txt}}
```
#### システムとファイルの非表示属性を削除します:
```shell
attrib -S -H {{ファイル名.txt}}
```
#### 非表示の属性をディレクトリに追加します:
```shell
attrib +H {{ディレクトリパス}}
```
{% endraw %}