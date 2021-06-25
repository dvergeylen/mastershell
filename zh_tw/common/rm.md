---
layout: default
title: "rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rm">
  <a href="/zh_tw/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 移除檔案或目錄。
> 更多資訊： <https://www.gnu.org/software/coreutils/rm>.

#### 移除位於指定路徑的檔案：
```shell
rm {{檔案一/完整/路徑}} {{檔案二/完整/路徑}}
```
#### 遞迴移除目錄與其所有子目錄：
```shell
rm -r {{目錄/完整/路徑}}
```
#### 強制移除目錄，且不會跳出任何確認資訊與錯誤訊息：
```shell
rm -rf {{目錄/完整/路徑}}
```
#### 移除檔案，且每次移除都會進行確認：
```shell
rm -i {{檔案一}} {{檔案二}}
```
#### 移除目錄中的所有檔案，並顯示每個檔案的移除資訊：
```shell
rm -v {{目錄/完整/路徑/*}}
```
{% endraw %}