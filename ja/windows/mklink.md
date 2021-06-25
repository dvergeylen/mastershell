---
layout: default
title: "mklink"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mklink">
  <a href="/ja/windows/mklink.html">mklink</a> <a href="#mklink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> シンボリックリンクを作成します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/mklink>.

#### ファイルへのシンボリックリンクを作成します:
```shell
mklink {{リンクパス}} {{ソースファイルのパス}}
```
#### ディレクトリへのシンボリックリンクを作成します:
```shell
mklink /d {{リンクパス}} {{ソースディレクトリパス}}
```
#### ファイルへのハードリンクを作成します:
```shell
mklink /h {{リンクパス}} {{ソースファイルのパス}}
```
#### ディレクトリジャンクションを作成します:
```shell
mklink /j {{リンクパス}} {{ソースファイルのパス}}
```
{% endraw %}