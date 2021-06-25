---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/zh_tw/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 連接檔案並印出檔案的內容。
> 更多資訊： <https://www.gnu.org/software/coreutils/cat>.

#### 將檔案的內容印在標準輸出：
```shell
cat {{檔案}}
```
#### 將多個檔案連接起來，輸出至目標檔案：
```shell
cat {{檔案一}} {{檔案二}} > {{目標檔案}}
```
#### 將多個檔案連接起來，並將其內容加到目標檔案的結尾：
```shell
cat {{檔案一}} {{檔案二}} >> {{目標檔案}}
```
#### 印出檔案的內容並顯示行號：
```shell
cat -n {{檔案}}
```
#### 印出檔案的內容，且將無法顯示的字元用特殊的方式顯示出來：
```shell
cat -v -t -e {{檔案}}
```
{% endraw %}