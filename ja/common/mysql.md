---
layout: default
title: "mysql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysql">
  <a href="/ja/common/mysql.html">mysql</a> <a href="#mysql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MySQL のコマンドラインツールです。
> 詳しくはこちら: <https://www.mysql.com/>.

#### データベースへの接続:
```shell
mysql {{データベース名}}
```
#### データベースへの接続、ユーザーにはパスワードの入力が求められる:
```shell
mysql -u {{ユーザー}} --password {{データベース名}}
```
#### 別のホスト上のデータベースに接続する:
```shell
mysql -h {{データベースホスト}} {{データベース名}}
```
#### Unix ソケット経由でのデータベースへの接続:
```shell
mysql --socket {{ソケットファイルへのパス}}
```
#### スクリプトファイル（バッチファイル）での SQL 文の実行:
```shell
mysql -e "source {{sqlファイル}}" {{データベース名}}
```
#### `mysqldump` で作成したバックアップからデータベースをリストアする（ユーザーはパスワードの入力を求められます）:
```shell
mysql --user {{ユーザー}} --password {{データベース名}} < {{バックアップsqlファイルへのパス}}
```
#### バックアップからすべてのデータベースを復元する（ユーザーはパスワードの入力を求められます）:
```shell
mysql --user {{ユーザー}} --password < {{バックアップsqlファイルへのパス}}
```
{% endraw %}