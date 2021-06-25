---
layout: default
title: "ranger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ranger">
  <a href="/ja/common/ranger.html">ranger</a> <a href="#ranger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> VI キーバインドのコンソールファイルマネージャー
> 詳しくはこちら: <https://github.com/ranger/ranger>.

#### ranger を起動する。
```shell
ranger
```
#### ディレクトリのみ表示する。
```shell
ranger --show-only-dirs
```
#### 設定ディレクトリを変更する。
```shell
ranger --confdir={{path/to/directory}}
```
#### データディレクトリを変更する。
```shell
ranger --datadir={{path/to/directory}}
```
#### 終了時に CPU 使用統計を表示する。
```shell
ranger --profile
```
{% endraw %}