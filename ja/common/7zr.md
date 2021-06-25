---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/ja/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 7-Zipは高圧縮率のファイルアーカイバ
> .7zファイルをアーカイブタイプをサポートする
> 詳しくはこちら: <https://sevenzip.osdn.jp/>.

#### ファイルまたはディレクトリをアーカイブする:
```shell
7zr a {{アーカイブ.7z}} {{道/に/ファイルまたはディレクトリ}}
```
#### 元のディレクトリ構造で既存の7zファイルを抽出します:
```shell
7zr x {{アーカイブ.7z}}
```
#### アーカイブの内容を一します:
```shell
7zr l {{アーカイブ.7z}}
```
{% endraw %}