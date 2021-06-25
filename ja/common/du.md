---
layout: default
title: "du"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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
{% endraw %}