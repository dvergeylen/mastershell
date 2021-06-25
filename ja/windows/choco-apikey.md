---
layout: default
title: "choco-apikey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-apikey">
  <a href="/ja/windows/choco-apikey.html">choco-apikey</a> <a href="#choco-apikey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ChocolateyソースのAPIキーを管理します
> 詳しくはこちら: <https://chocolatey.org/docs/commands-apikey>.

#### ソースとそのAPIキーのリストを表示します:
```shell
choco apikey
```
#### 特定のソースとそのAPIキーを表示します:
```shell
choco apikey --source "{{ソースURL}}"
```
#### ソースのAPIキーを設定します:
```shell
choco apikey --source "{{ソースURL}}" --key "{{APIキー}}"
```
#### ソースのAPIキーを削除します:
```shell
choco apikey --source "{{ソースURL}}" --remove
```
{% endraw %}