---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/ja/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ディレクトリの内容を一覧表示します。
> 詳しくはこちら: <https://www.gnu.org/software/coreutils/ls>.

#### ファイルを1行ごとに一覧表示:
```shell
ls -1
```
#### 隠しファイルを含むすべてのファイルを一覧表示:
```shell
ls -a
```
#### すべてのファイルを一覧表示し、ディレクトリ名の最後に `/` を付加する:
```shell
ls -F
```
#### 全ファイルを長い形式（パーミッション、所有者、サイズ、修正日）で一覧表示します:
```shell
ls -la
```
#### サイズを人間が読みやすい単位（KiB、MiB、GiB）で表示した長い形式での一覧表示:
```shell
ls -lh
```
#### サイズ順（降順）に並べた長い形式での一覧表示:
```shell
ls -lS
```
#### すべてのファイルの長い形式でのリストで、更新日が古いものから順に表示されます:
```shell
ls -ltr
```
{% endraw %}