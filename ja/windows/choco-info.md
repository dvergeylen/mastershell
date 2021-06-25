---
layout: default
title: "choco info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-info">
  <a href="/ja/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chocolateyのパッケージに関する詳細情報を表示します
> 詳しくはこちら: <https://chocolatey.org/docs/commands-info>.

#### 特定のパッケージに関する情報を表示します:
```shell
choco info {{パッケージ}}
```
#### ローカルパッケージ情報のみを表示します:
```shell
choco info {{パッケージ}} --local-only
```
#### パッケージ情報を受信するカスタムソースを指定します:
```shell
choco info {{パッケージ}} --source {{ソースURL|エイリアス}}
```
#### 認証用のユーザー名とパスワードを入力します:
```shell
choco info {{パッケージ}} --user {{ユーザー名}} --password {{パスワード}}
```
{% endraw %}