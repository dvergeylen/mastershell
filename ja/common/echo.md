---
layout: default
title: "echo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="echo">
  <a href="/ja/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 与えられた引数を表示します。
> 詳しくはこちら: <https://www.gnu.org/software/coreutils/echo>.

#### テキストメッセージを印刷する。備考: 引用符は任意:
```shell
echo "{{Hello World}}"
```
#### 環境変数のメッセージを表示する:
```shell
echo "{{パスは $PATH です。}}"
```
#### メッセージを最後の改行なしで表示する:
```shell
echo -n "{{Hello World}}"
```
#### ファイルにメッセージを追加する:
```shell
echo "{{Hello World}}" >> {{ファイル.txt}}
```
#### バックスラッシュエスケープ（特殊文字）の解釈を可能にする:
```shell
echo -e "{{カラム 1\tカラム 2}}"
```
{% endraw %}