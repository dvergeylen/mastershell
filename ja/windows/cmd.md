---
layout: default
title: "cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmd">
  <a href="/ja/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windowsコマンドインタープリター
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/cmd>.

#### コマンドインタープリターの新しいインスタンスを開始します:
```shell
cmd
```
#### 指定されたコマンドを実行して終了します:
```shell
cmd /c "{{コマンド}}"
```
#### 指定されたコマンドを実行して、インタラクティブシェルに入ります:
```shell
cmd /k "{{コマンド}}"
```
#### コマンドの出力での「echo」の使用を無効にします:
```shell
cmd /q
```
#### コマンド拡張機能を有効または無効にします:
```shell
cmd /e:{{on|off}}
```
#### ファイルまたはディレクトリのオートコンプリートを有効または無効にします:
```shell
cmd /f:{{on|off}}
```
#### 環境変数の拡張を有効または無効にします:
```shell
cmd /v:{{on|off}}
```
#### 出力でUnicodeエンコーディングを使用するように強制します:
```shell
cmd /u
```
{% endraw %}