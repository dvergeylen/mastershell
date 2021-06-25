---
layout: default
title: "z"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="z">
  <a href="/ja/common/z.html">z</a> <a href="#z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 高頻度で利用されるディレクトリを把握し、文字列や正規表現をつかうことでスムーズに移動できるようにします。
> 詳しくはこちら: <https://github.com/rupa/z>.

#### "foo"が名前に含まれるディレクトリに移動する。
```shell
z {{foo}}
```
#### "foo"と"bar"が名前に含まれるディレクトリに移動する。
```shell
z {{foo}} {{bar}}
```
#### "foo"と最もマッチングするディレクトリに移動する。
```shell
z -r {{foo}}
```
#### "foo"とマッチングするディレクトリの中で、最も最近アクセスしたディレクトリに移動する。
```shell
z -t {{foo}}
```
#### `z`コマンドのデータベースの中で、`foo` にマッチングするディレクトリの一覧を表示する。
```shell
z -l {{foo}}
```
#### 現在のディレクトリを`z`コマンドのデータベース除去する。
```shell
z -x .
```
{% endraw %}