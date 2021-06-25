---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#7z">7z</a>
* <a href="#7za">7za</a>
* <a href="#7zr">7zr</a>
* <a href="#arch">arch</a>
* <a href="#cp">cp</a>
* <a href="#dig">dig</a>
* <a href="#du">du</a>
* <a href="#echo">echo</a>
* <a href="#less">less</a>
* <a href="#ls">ls</a>
* <a href="#mysql">mysql</a>
* <a href="#ps">ps</a>
* <a href="#pwd">pwd</a>
* <a href="#ranger">ranger</a>
* <a href="#sed">sed</a>
* <a href="#tar">tar</a>
* <a href="#tldr">tldr</a>
* <a href="#vim">vim</a>
* <a href="#z">z</a>

{% raw %}
<h2 id="7z">
  <a href="/ja/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 7-Zipは高圧縮率のファイルアーカイバ
> 詳しくはこちら: <https://sevenzip.osdn.jp/>.

#### ファイルまたはディレクトリをアーカイブする:
```shell
7z a {{アーカイブ.7z}} {{道/に/ファイルまたはディレクトリ}}
```
#### 既存のアーカイブを暗号 (ヘッダーを含む):
```shell
7z a {{暗号する.7z}} -p{{パスワード}} -mhe=on {{アーカイブ.7z}}
```
#### 元のディレクトリ構造で既存の7zファイルを抽出します:
```shell
7z x {{アーカイブ.7z}}
```
#### ユーザー定義の出力パスで既存の7zファイルを抽出します:
```shell
7z x {{アーカイブ.7z}} -o{{道/に/出力}}
```
#### stdoutの出力で既存のファイルを抽出します:
```shell
7z x {{アーカイブ.7z}} -so
```
#### 特定のアーカイブタイプを使用したアーカイブする:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{アーカイブ.7z}} {{道/に/ファイルまたはディレクトリ}}
```
#### 利用可能なアーカイブプをします:
```shell
7z i
```
#### アーカイブの内容を一します:
```shell
7z l {{アーカイブ.7z}}
```
{% endraw %}{% raw %}
<h2 id="7za">
  <a href="/ja/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 7-Zipは高圧縮率のファイルアーカイバ
> より少ないアーカイブタイプをサポートする `7z`. スタンドアロンバージョン.
> 詳しくはこちら: <https://sevenzip.osdn.jp/>.

#### ファイルまたはディレクトリをアーカイブする:
```shell
7za a {{アーカイブ.7z}} {{道/に/ファイルまたはディレクトリ}}
```
#### 元のディレクトリ構造で既存の7zファイルを抽出します:
```shell
7za x {{アーカイブ}}
```
#### 特定のアーカイブタイプを使用したアーカイブする:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{アーカイブ}} {{道/に/ファイルまたはディレクトリ}}
```
#### 利用可能なアーカイブプをします:
```shell
7za i
```
#### アーカイブの内容を一します:
```shell
7za l {{アーカイブ}}
```
{% endraw %}{% raw %}
<h2 id="7zr">
  <a href="/ja/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 7-Zipは高圧縮率のファイルアーカイバ
> .7zファイルをアーカイブタイプをサポートする
> 詳しくはこちら: <https://sevenzip.osdn.jp/>.

#### ファイルまたはディレクトリをアーカイブする:
```shell
7zr a {{アーカイブ.7z}} {{道/に/ファイルまたはディレクトリ}}
```
#### 元のディレクトリ構造で既存の7zファイルを抽出します:
```shell
7zr x {{アーカイブ.7z}}
```
#### アーカイブの内容を一します:
```shell
7zr l {{アーカイブ.7z}}
```
{% endraw %}{% raw %}
<h2 id="arch">
  <a href="/ja/common/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> システムアーキテクチャ名前を示する.
> 'uname' も参照してください.
> 詳しくはこちら: <https://www.gnu.org/software/coreutils/arch>.

#### システムアーキテクチャを示する:
```shell
arch
```
{% endraw %}{% raw %}
<h2 id="cp">
  <a href="/ja/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ファイルやディレクトリをコピーします。
> 詳しくはこちら: <https://www.gnu.org/software/coreutils/cp>.

#### ファイルを別の場所にコピー:
```shell
cp {{コピー元ファイルへのパス}} {{コピー先ファイルへのパス}}
```
#### ファイル名を維持したまま、ファイルを別のディレクトリにコピーする:
```shell
cp {{コピー元ファイルへのパス}} {{コピー先ディレクトリへのパス}}
```
#### ディレクトリの内容を別の場所に再帰的にコピーする（コピー先が存在する場合は、その中にディレクトリがコピーされる):
```shell
cp -R {{コピー元ディレクトリへのパス}} {{コピー先ディレクトリへのパス}}
```
#### 詳細モードでディレクトリを再帰的にコピーする（コピーされたファイルが表示される）:
```shell
cp -vR {{コピー元ディレクトリへのパス}} {{コピー先ディレクトリへのパス}}
```
#### 対話形式でテキストファイルを別の場所にコピーする（上書きする前にユーザーに確認する）:
```shell
cp -i {{*.txt}} {{コピー先ディレクトリへのパス}}
```
#### コピーする前にシンボリックリンクをたどる:
```shell
cp -L {{link}} {{コピー先ディレクトリへのパス}}
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="du">
  <a href="/ja/common/du.html">du</a> <a href="#du"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ディスク使用状況: ファイルとディレクトリの使用量の概算を表示します。
> 詳しくはこちら: <https://www.gnu.org/software/coreutils/du>.

#### 指定した単位(B/KB/MB)でディレクトリおよびサブディレクトリのサイズを表示します。
```shell
du -{{b|k|m}} {{path/to/directory}}
```
#### 人間にとって解釈しやすい形式(サイズに応じた単位の選択など)で、ディレクトリおよびサブディレクトリのサイズを表示します。
```shell
du -h {{path/to/directory}}
```
#### 人間にとって解釈しやすい形式で、単一ディレクトリのサイズを表示します。
```shell
du -sh {{path/to/directory}}
```
#### 人間にとって解釈しやすい形式で、指定ディレクトリ、そのサブディレクトリ、それらに含まれる全てのファイルのサイズを表示します。
```shell
du -ah {{path/to/directory}}
```
#### 人間にとって解釈しやすい形式で、指定ディレクトリおよび N 階層先までのディレクトリのサイズを表示します。
```shell
du -h --max-depth=N {{path/to/directory}}
```
#### 人間にとって解釈しやすい形式で、現在のディレクトリおよびその下のディレクトリに含まれる全ての `.jpg` ファイルサイズを表示し、最後に合計を表示します。
```shell
du -ch */*.jpg
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="less">
  <a href="/ja/common/less.html">less</a> <a href="#less"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ファイルを開いて、スクロールや検索などのインタラクティブな読み方ができます。
> 詳しくはこちら: <https://greenwoodsoftware.com/less/>.

#### ファイルを開く:
```shell
less {{ソースファイル}}
```
#### ページダウン/アップ:
```shell
<スペース> (ダウン), b (アップ)
```
#### ファイルの最後/最初に移動:
```shell
G (最後), g (最初)
```
#### 文字列の前方検索（`n`/`N` を押すと、次の/前のマッチに移動する）:
```shell
/{{検索文字列}}
```
#### 文字列の後方検索（`n`/`N` を押すと次/前のマッチに進む）:
```shell
?{{検索文字列}}
```
#### 現在開いているファイルの出力を追跡する:
```shell
F
```
#### 現在のファイルをエディターで開く:
```shell
v
```
#### 閉じる:
```shell
q
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/ja/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ディレクトリの内容を一覧表示します。
> 詳しくはこちら: <https://www.gnu.org/software/coreutils/ls>.

#### ファイルを1行ごとに一覧表示:
```shell
ls -1
```
#### 隠しファイルを含むすべてのファイルを一覧表示:
```shell
ls -a
```
#### すべてのファイルを一覧表示し、ディレクトリ名の最後に `/` を付加する:
```shell
ls -F
```
#### 全ファイルを長い形式（パーミッション、所有者、サイズ、修正日）で一覧表示します:
```shell
ls -la
```
#### サイズを人間が読みやすい単位（KiB、MiB、GiB）で表示した長い形式での一覧表示:
```shell
ls -lh
```
#### サイズ順（降順）に並べた長い形式での一覧表示:
```shell
ls -lS
```
#### すべてのファイルの長い形式でのリストで、更新日が古いものから順に表示されます:
```shell
ls -ltr
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="ps">
  <a href="/ja/common/ps.html">ps</a> <a href="#ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 実行中のプロセスに関する情報。

#### 実行中のプロセスをすべてリストアップ:
```shell
ps aux
```
#### 実行中のすべてのプロセスを、完全なコマンド文字列を含めて一覧表示する:
```shell
ps auxww
```
#### 文字列にマッチするプロセスを検索する:
```shell
ps aux | grep {{文字列}}
```
#### 現在のユーザーのすべてのプロセスを完全なフォーマットで表示する:
```shell
ps --user $(id -u) -F
```
#### カレントユーザーの全プロセスをツリー状にリストアップ:
```shell
ps --user $(id -u) f
```
#### プロセスの親 pid を取得する:
```shell
ps -o ppid= -p {{pid}}
```
#### プロセスをメモリ消費量でソート:
```shell
ps --sort size
```
{% endraw %}{% raw %}
<h2 id="pwd">
  <a href="/ja/common/pwd.html">pwd</a> <a href="#pwd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 現在の作業ディレクトリを表示します。
> 詳しくはこちら: <https://www.gnu.org/software/coreutils/pwd>.

#### 現在のディレクトリを表示する:
```shell
pwd
```
#### 現在のディレクトリを表示し、すべてのシンボリックリンクを解決する（つまり、「物理的な」パスを表示する）:
```shell
pwd -P
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="sed">
  <a href="/ja/common/sed.html">sed</a> <a href="#sed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> スクリプトによるテキスト編集。
> 詳しくはこちら: <https://man.archlinux.org/man/sed.1>.

#### ファイルの各行で正規表現の最初の出現箇所を置換し、その結果を表示する:
```shell
sed 's/{{正規表現}}/{{置き換え後}}/' {{ファイル名}}
```
#### ファイル内の拡張正規表現のすべての出現箇所を置換し、その結果を表示する:
```shell
sed -r 's/{{正規表現}}/{{置き換え後}}/g' {{ファイル名}}
```
#### ファイル内のすべての文字列を置き換え、ファイルを上書きする(すなわち インプレイス):
```shell
sed -i 's/{{置き換え前}}/{{置き換え後}}/g' {{ファイル名}}}
```
#### ラインパターンに一致する行のみを置換:
```shell
sed '/{{ラインパターン}}/s/{{置き換え前}}/{{置き換え後}}/' {{ファイル名}}
```
#### ラインパターンに一致する行を削除する:
```shell
sed '/{{ラインパターン}}/d' {{ファイル名}}}
```
#### ファイルの最初の 11 行を表示する:
```shell
sed 11q {{ファイル名}}
```
#### 複数の検索・置換式をファイルに適用:
```shell
sed -e 's/{{置き換え名}}/{{置き換え後}}/' -e 's/{{置き換え前}}/{{置き換え後}}/' {{ファイル名}}
```
#### 区切り文字 `/` を、検索や置換のパターンで使われていない他の文字（例：`#`）で置き換える:
```shell
sed 's#{{置き換え前}}#{{置き換え後}}#' {{ファイル名}}
```
{% endraw %}{% raw %}
<h2 id="tar">
  <a href="/ja/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> アーカイブ(複数のファイルやフォルダを 1 つのファイルに纏める)の為のユーティリティー。
> gzip や bzip2 などの圧縮方法と組み合わせることが多いです。
> 詳しくはこちら: <https://www.gnu.org/software/tar>.

#### アーカイブを作成し、それをファイルに書き込む:
```shell
tar cf {{出力ファイル名.tar}} {{ファイル1}} {{ファイル2}} {{ファイル3}}
```
#### gzip 形式で圧縮されたアーカイブを作成し、それをファイルに書き込む:
```shell
tar czf {{出力ファイル名.tar.gz}} {{ファイル1}} {{ファイル2}} {{ファイル3}}
```
#### 相対パスを用いてディレクトリから gzip 形式のアーカイブを作成する:
```shell
tar czf {{出力ファイル名.tar.gz}} --directory={{ディレクトリへの相対パス}} .
```
#### (圧縮された)アーカイブファイルを、カレントディレクトリに過程を詳細表示しながら展開する:
```shell
tar xvf {{入力ファイル名.tar[.gz|.bz2|.xz]}}
```
#### (圧縮された)アーカイブファイルを、指定のディレクトリに展開する:
```shell
tar xf {{入力ファイル名.tar[.gz|.bz2|.xz]}} --directory={{ディレクトリ}}
```
#### 圧縮されたアーカイブを作成し、それにファイルを書き込む。なお、接尾辞で圧縮プログラムを指定する:
```shell
tar caf {{出力ファイル名.tar.xz}} {{ファイル1}} {{ファイル2}} {{ファイル3}}
```
#### tar ファイルの内容を詳細に表示する:
```shell
tar tvf {{入力ファイル名.tar}}
```
#### アーカイブファイルからパターンに合致するファイルを抽出する:
```shell
tar xf {{入力ファイル名.tar}} --wildcards "{{*.html}}"
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/ja/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> コマンドの簡単なマニュアル
> 詳しくはこちら: <https://tldr.sh>.

#### コマンドのよくある使用例を見られます (ヒント: このページにたどり着いた方法です！):
```shell
tldr {{コマンド}}
```
#### tarのlinux向けtldrページを見る:
```shell
tldr -p {{linux}} {{tar}}
```
#### gitのサブコマンドについての情報を見る:
```shell
tldr {{git checkout}}
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="z">
  <a href="/ja/common/z.html">z</a> <a href="#z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 高頻度で利用されるディレクトリを把握し、文字列や正規表現をつかうことでスムーズに移動できるようにします。
> 詳しくはこちら: <https://github.com/rupa/z>.

#### "foo"が名前に含まれるディレクトリに移動する。
```shell
z {{foo}}
```
#### "foo"と"bar"が名前に含まれるディレクトリに移動する。
```shell
z {{foo}} {{bar}}
```
#### "foo"と最もマッチングするディレクトリに移動する。
```shell
z -r {{foo}}
```
#### "foo"とマッチングするディレクトリの中で、最も最近アクセスしたディレクトリに移動する。
```shell
z -t {{foo}}
```
#### `z`コマンドのデータベースの中で、`foo` にマッチングするディレクトリの一覧を表示する。
```shell
z -l {{foo}}
```
#### 現在のディレクトリを`z`コマンドのデータベース除去する。
```shell
z -x .
```
{% endraw %}