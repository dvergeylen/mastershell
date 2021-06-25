---
layout: default
title: "ps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ps">
  <a href="/ja/common/ps.html">ps</a> <a href="#ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 実行中のプロセスに関する情報。

#### 実行中のプロセスをすべてリストアップ:
```shell
ps aux
```
#### 実行中のすべてのプロセスを、完全なコマンド文字列を含めて一覧表示する:
```shell
ps auxww
```
#### 文字列にマッチするプロセスを検索する:
```shell
ps aux | grep {{文字列}}
```
#### 現在のユーザーのすべてのプロセスを完全なフォーマットで表示する:
```shell
ps --user $(id -u) -F
```
#### カレントユーザーの全プロセスをツリー状にリストアップ:
```shell
ps --user $(id -u) f
```
#### プロセスの親 pid を取得する:
```shell
ps -o ppid= -p {{pid}}
```
#### プロセスをメモリ消費量でソート:
```shell
ps --sort size
```
{% endraw %}