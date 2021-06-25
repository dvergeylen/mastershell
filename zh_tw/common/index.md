---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#cat">cat</a>
* <a href="#cd">cd</a>
* <a href="#echo">echo</a>
* <a href="#ls">ls</a>
* <a href="#mkdir">mkdir</a>
* <a href="#pwd">pwd</a>
* <a href="#rm">rm</a>
* <a href="#rmdir">rmdir</a>
* <a href="#tldr">tldr</a>
* <a href="#touch">touch</a>

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
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/zh_tw/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 改變工作目錄。
> 更多資訊： <https://man.archlinux.org/man/cd.n>.

#### 前往指定目錄：
```shell
cd {{目錄/完整/路徑}}
```
#### 前往目前使用者的家目錄：
```shell
cd
```
#### 前往目前目錄的上層目錄：
```shell
cd ..
```
#### 前往之前所在的目錄：
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="echo">
  <a href="/zh_tw/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 印出文字。
> 更多資訊： <https://www.gnu.org/software/coreutils/echo>.

#### 印出一行文字（如果文字中沒有連續的空格，可以不加引號）：
```shell
echo "{{文字}}"
```
#### 印出包含環境變數的文字：
```shell
echo "{{我的家目錄位於 $HOME}}"
```
#### 印出文字，但結尾不換行：
```shell
echo -n "{{文字}}"
```
#### 將一段文字加到檔案的結尾：
```shell
echo "{{文字}}" >> {{檔案}}
```
#### 將以「\\」開頭的跳脫序列轉換為特殊字元（例如「\t」會被顯示為水平定位字元）：
```shell
echo -e "{{第一欄\t第二欄}}"
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/zh_tw/common/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 建立目錄。
> 更多資訊： <https://www.gnu.org/software/coreutils/mkdir>.

#### 在目前所在目錄或指定路徑中建立新目錄：
```shell
mkdir {{目錄/完整/路徑}}
```
#### 遞迴建立目錄，若上層目錄尚未被建立則會一併建立：
```shell
mkdir -p {{目錄/完整/路徑}}
```
{% endraw %}{% raw %}
<h2 id="pwd">
  <a href="/zh_tw/common/pwd.html">pwd</a> <a href="#pwd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 印出目前目錄的名稱。
> 更多資訊： <https://www.gnu.org/software/coreutils/pwd>.

#### 印出目前所在的目錄名稱：
```shell
pwd
```
#### 印出目前所在的目錄名稱，並將符號連結轉換為實體路徑：
```shell
pwd -P
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="rmdir">
  <a href="/zh_tw/common/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 移除目錄。
> 更多資訊： <https://www.gnu.org/software/coreutils/rmdir>.

#### 若為空目錄則移除目錄（如果目錄非空，可用 `rm -r` 移除目錄及其所包含的檔案）：
```shell
rmdir {{目錄/完整/路徑}}
```
#### 移除目錄與其所有上層目錄：
```shell
rmdir -p {{目錄/完整/路徑}}
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/zh_tw/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 由 tldr-pages 專案所提供的簡單版指令簡介。
> 更多資訊：<https://tldr.sh>.

#### 顯示指令的常用用法：
```shell
tldr {{指令}}
```
#### 顯示 Linux 作業系統中 tar 指令的用法：
```shell
tldr -p {{linux}} {{tar}}
```
#### 顯示 Git 的子指令 checkout 的用法：
```shell
tldr {{git-checkout}}
```
{% endraw %}{% raw %}
<h2 id="touch">
  <a href="/zh_tw/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 改變檔案的存取與修改時間。
> 更多資訊： <https://www.gnu.org/software/coreutils/touch>.

#### 建立新檔案，或更新現存檔案的存取與修改時間：
```shell
touch {{檔案名稱}}
```
#### 將存取與修改時間設定為指定時刻：
```shell
touch -t {{西元年份月份日期小時分鐘.秒鐘}} {{檔案名稱}}
```
#### 以其中一個檔案的存取與修改時間為基準，設定另一個檔案的存取與修改時間：
```shell
touch -r {{來源檔案名稱}} {{目標檔案名稱}}
```
{% endraw %}