---
layout: default
title: "touch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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