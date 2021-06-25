---
layout: default
title: "assoc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="assoc">
  <a href="/ja/windows/assoc.html">assoc</a> <a href="#assoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ファイル拡張子の関連付けを表示または変更します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/assoc>.

#### 関連するすべてのファイルタイプをします:
```shell
assoc
```
#### 特定の拡張子に関連付けられているファイルの種類を表示します:
```shell
assoc {{.txt}}
```
#### 特定の拡張子に関連付けられたファイルタイプを変更します:
```shell
assoc {{.txt}}={{テキストファイル}}
```
{% endraw %}