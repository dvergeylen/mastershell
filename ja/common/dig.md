---
layout: default
title: "dig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dig">
  <a href="/ja/common/dig.html">dig</a> <a href="#dig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DNS 情報を調べるユーティリティーです。
> 詳しくはこちら: <https://manpages.debian.org/dnsutils/dig.1.html>.

#### ホスト名に関連する IP を検索（A レコード）:
```shell
dig +short {{example.com}}
```
#### 指定したドメインの詳細な回答を得る（A レコード）:
```shell
dig +noall +answer {{example.com}}
```
#### 指定されたドメイン名に関連する特定の DNS レコードタイプを取得する:
```shell
dig +short {{example.com}} {{A|MX|TXT|CNAME|NS}}
```
#### 指定したドメイン名のすべてのタイプのレコードを取得する:
```shell
dig {{example.com}} ANY
```
#### 問い合わせる別の DNS サーバーを指定する:
```shell
dig @{{8.8.8.8}} {{example.com}}
```
#### IP アドレスの DNS 逆引きの実行（PTR レコード）:
```shell
dig -x {{8.8.8.8}}
```
#### ゾーンの権威ネームサーバーの検索と SOA レコードの表示:
```shell
dig +nssearch {{example.com}}
```
#### ドメイン名を解決するための反復的なクエリの実行と、そのトレースパス全体を表示する:
```shell
dig +trace {{example.com}}
```
{% endraw %}