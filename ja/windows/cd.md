---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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
{% endraw %}