---
layout: default
title: "less"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="less">
  <a href="/ja/common/less.html">less</a> <a href="#less"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ファイルを開いて、スクロールや検索などのインタラクティブな読み方ができます。
> 詳しくはこちら: <https://greenwoodsoftware.com/less/>.

#### ファイルを開く:
```shell
less {{ソースファイル}}
```
#### ページダウン/アップ:
```shell
<スペース> (ダウン), b (アップ)
```
#### ファイルの最後/最初に移動:
```shell
G (最後), g (最初)
```
#### 文字列の前方検索（`n`/`N` を押すと、次の/前のマッチに移動する）:
```shell
/{{検索文字列}}
```
#### 文字列の後方検索（`n`/`N` を押すと次/前のマッチに進む）:
```shell
?{{検索文字列}}
```
#### 現在開いているファイルの出力を追跡する:
```shell
F
```
#### 現在のファイルをエディターで開く:
```shell
v
```
#### 閉じる:
```shell
q
```
{% endraw %}