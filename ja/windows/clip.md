---
layout: default
title: "clip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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
{% endraw %}