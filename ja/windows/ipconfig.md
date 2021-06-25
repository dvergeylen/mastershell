---
layout: default
title: "ipconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipconfig">
  <a href="/ja/windows/ipconfig.html">ipconfig</a> <a href="#ipconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windowsのネットワーク構成を表示および管理します。
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/ipconfig>.

#### ネットワークアダプタのリストを表示します:
```shell
ipconfig
```
#### ネットワークアダプタの詳細なリストを表示します:
```shell
ipconfig /all
```
#### ネットワークアダプタのIPアドレスを更新します:
```shell
ipconfig /renew {{adapter}}
```
#### ネットワークアダプタのIPアドレスを解放します:
```shell
ipconfig /release {{adapter}}
```
#### DNSキャッシュからすべてのデータを削除します:
```shell
ipconfig /flushdns
```
{% endraw %}