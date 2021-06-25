---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/zh_tw/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 列出目錄內容。
> 更多資訊： <https://www.gnu.org/software/coreutils/ls>.

#### 列出目錄中的檔案，其中每個檔案佔一行：
```shell
ls -1
```
#### 列出包含隱藏檔案的所有檔案：
```shell
ls -a
```
#### 列出檔案，並依照檔案類型在檔案後面加上對應的符號（例如目錄會加上「/」）：
```shell
ls -F
```
#### 列出包含隱藏檔案的完整檔案列表（包括權限、擁有者、檔案大小與修改日期）：
```shell
ls -la
```
#### 列出完整檔案列表，其中檔案大小會用 KiB、MiB、GiB 表示：
```shell
ls -lh
```
#### 列出完整檔案列表，並依檔案大小降序排序：
```shell
ls -lS
```
#### 列出完整檔案列表，並依修改時間由舊到新排序：
```shell
ls -ltr
```
{% endraw %}