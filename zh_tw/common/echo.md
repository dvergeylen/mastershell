---
layout: default
title: "echo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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
{% endraw %}