---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#assoc">assoc</a>
* <a href="#attrib">attrib</a>
* <a href="#cd">cd</a>
* <a href="#choco">choco</a>
* <a href="#choco-feature">choco feature</a>
* <a href="#choco-info">choco info</a>
* <a href="#choco-apikey">choco-apikey</a>
* <a href="#clip">clip</a>
* <a href="#cls">cls</a>
* <a href="#cmd">cmd</a>
* <a href="#dir">dir</a>
* <a href="#find">find</a>
* <a href="#ipconfig">ipconfig</a>
* <a href="#mkdir">mkdir</a>
* <a href="#mklink">mklink</a>

{% raw %}
<h2 id="assoc">
  <a href="/ja/windows/assoc.html">assoc</a> <a href="#assoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ファイル拡張子の関連付けを表示または変更します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/assoc>.

#### 関連するすべてのファイルタイプをします:
```shell
assoc
```
#### 特定の拡張子に関連付けられているファイルの種類を表示します:
```shell
assoc {{.txt}}
```
#### 特定の拡張子に関連付けられたファイルタイプを変更します:
```shell
assoc {{.txt}}={{テキストファイル}}
```
{% endraw %}{% raw %}
<h2 id="attrib">
  <a href="/ja/windows/attrib.html">attrib</a> <a href="#attrib"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ファイルまたはディレクトリの属性を表示または変更します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/attrib>.

#### 現在のディレクトリ内のファイルの属性を表示します:
```shell
attrib
```
#### 現在のディレクトリとサブディレクトリにあるファイルの属性を表示します:
```shell
attrib /S
```
#### 現在のディレクトリとサブディレクトリ内のファイルとディレクトリの属性を表示します:
```shell
attrib /S /D
```
#### ファイルに読み取り専用属性を追加します:
```shell
attrib +R {{ファイル名.txt}}
```
#### システムとファイルの非表示属性を削除します:
```shell
attrib -S -H {{ファイル名.txt}}
```
#### 非表示の属性をディレクトリに追加します:
```shell
attrib +H {{ディレクトリパス}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/ja/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 現在の作業ディレクトリの名前を表示するか、現在の作業ディレクトリを変更します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### 同じドライブ内のディレクトリに移動します:
```shell
cd {{ディレクトリパス}}
```
#### 現在のディレクトリの名前を表示します:
```shell
cd
```
#### 現在のディレクトリの親に移動します:
```shell
cd ..
```
#### 別のドライブのディレクトリに移動します:
```shell
cd {{ディレクトリパス}} /d
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="choco-feature">
  <a href="/ja/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chocolateyで機能を操作します.
> 詳しくはこちら: <https://chocolatey.org/docs/commands-feature>.

#### 利用可能な機能のリストを表示します:
```shell
choco feature list
```
#### 機能を有効にします:
```shell
choco feature enable --name {{名}}
```
#### 機能を無効にします:
```shell
choco feature disable --name {{名}}
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="choco">
  <a href="/ja/windows/choco.html">choco</a> <a href="#choco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chocolateyパッケージマネージャーのコマンドラインインターフェイスです
> 詳細については、「choco install」、「choco upgrade」などのページを参照してください
> 詳しくはこちら: <https://chocolatey.org>.

#### Chocolateyコマンドを実行します:
```shell
choco {{コマンド}}
```
#### 一般的なヘルプを表示します:
```shell
choco -?
```
#### 特定のコマンドのヘルプを表示します:
```shell
choco {{コマンド}} -?
```
#### Chocolateyバージョンを表示します:
```shell
choco --version
```
{% endraw %}{% raw %}
<h2 id="clip">
  <a href="/ja/windows/clip.html">clip</a> <a href="#clip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 入力コンテンツをWindowsクリップボードにコピーします
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/clip>.

#### コマンドライン出力をWindowsクリップボードにパイプします:
```shell
{{dir}} | clip
```
#### ファイルの内容をWindowsクリップボードにコピーします:
```shell
clip < {{path/to/file.ext}}
```
#### 末尾に改行が付いたテキストをWindowsクリップボードにコピーします:
```shell
echo {{テキスト}} | clip
```
#### 末尾の改行なしでテキストをWindowsクリップボードにコピーします:
```shell
echo | set /p="テキスト" | clip
```
{% endraw %}{% raw %}
<h2 id="cls">
  <a href="/ja/windows/cls.html">cls</a> <a href="#cls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 画面をクリアします
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/cls>.

#### 画面をクリアします:
```shell
cls
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="dir">
  <a href="/ja/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ディレクトリの内容を一覧表示します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### 現在のディレクトリの内容を表示します:
```shell
dir
```
#### 特定のディレクトリの内容を表示します:
```shell
dir {{ディレクトリパス}}
```
#### 非表示の内容を含む、現在のディレクトリの内容を表示します:
```shell
dir /A
```
#### 非表示の内容を含む、特定のディレクトリの内容を表示します:
```shell
dir {{ディレクトリパス}} /A
```
{% endraw %}{% raw %}
<h2 id="find">
  <a href="/ja/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 1つ以上のファイルで指定された文字列を検索します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### 指定された文字列を含む行を検索します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}}
```
#### 指定された文字列を含まない行を表示します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}} /v
```
#### 指定された文字列を含む行数を表示します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}} /c
```
#### 行リストとともに行番号を表示します:
```shell
find {{文字列}} {{ファイルまたはディレクトリのパス}} /n
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/ja/windows/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ディレクトリを作成します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/mkdir>.

#### ディレクトリを作成します:
```shell
mkdir {{ディレクトリ名}}
```
#### ネストされたディレクトリツリーを再帰的に作成します:
```shell
mkdir {{サブディレクトリ名のパス}}
```
{% endraw %}{% raw %}
<h2 id="mklink">
  <a href="/ja/windows/mklink.html">mklink</a> <a href="#mklink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> シンボリックリンクを作成します
> 詳しくはこちら: <https://docs.microsoft.com/windows-server/administration/windows-commands/mklink>.

#### ファイルへのシンボリックリンクを作成します:
```shell
mklink {{リンクパス}} {{ソースファイルのパス}}
```
#### ディレクトリへのシンボリックリンクを作成します:
```shell
mklink /d {{リンクパス}} {{ソースディレクトリパス}}
```
#### ファイルへのハードリンクを作成します:
```shell
mklink /h {{リンクパス}} {{ソースファイルのパス}}
```
#### ディレクトリジャンクションを作成します:
```shell
mklink /j {{リンクパス}} {{ソースファイルのパス}}
```
{% endraw %}