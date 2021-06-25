---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/ja/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 7-Zipは高圧縮率のファイルアーカイバ
> より少ないアーカイブタイプをサポートする `7z`. スタンドアロンバージョン.
> 詳しくはこちら: <https://sevenzip.osdn.jp/>.

#### ファイルまたはディレクトリをアーカイブする:
```shell
7za a {{アーカイブ.7z}} {{道/に/ファイルまたはディレクトリ}}
```
#### 元のディレクトリ構造で既存の7zファイルを抽出します:
```shell
7za x {{アーカイブ}}
```
#### 特定のアーカイブタイプを使用したアーカイブする:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{アーカイブ}} {{道/に/ファイルまたはディレクトリ}}
```
#### 利用可能なアーカイブプをします:
```shell
7za i
```
#### アーカイブの内容を一します:
```shell
7za l {{アーカイブ}}
```
{% endraw %}