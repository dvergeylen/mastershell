---
layout: default
title: "vim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vim">
  <a href="/ja/common/vim.html">vim</a> <a href="#vim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> コマンドラインのテキストエディタである Vim（Vi IMproved）には、さまざまな種類のテキスト操作のためのモードが用意されています。
> `i` を押すと編集モードになります。`<Esc>` を押すと通常モードに戻り、通常のテキスト挿入はできません。
> 詳細はこちら: <https://www.vim.org>.

#### ファイルを開く:
```shell
vim {{ファイルへのパス}}
```
#### Vim のヘルプマニュアルを見る:
```shell
:help<Enter>
```
#### 保存と終了:
```shell
:wq<Enter>
```
#### 指定した行番号でファイルを開く:
```shell
vim +{{ライン番号}} {{ファイルへのパス}}
```
#### 最後の操作を元に戻す:
```shell
u
```
#### ファイル内のパターンを検索する（`n`/`N` を押すと次/前のマッチに進む）:
```shell
/{{検索パターン}}<Enter>
```
#### ファイル全体での正規表現による置換の実行:
```shell
:%s/{{パターン}}/{{置き換え後}}/g<Enter>
```
#### ライン番号の表示:
```shell
:set nu<Enter>
```
{% endraw %}