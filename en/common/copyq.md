---
layout: default
title: "copyq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="copyq">
  <a href="/en/common/copyq.html">copyq</a> <a href="#copyq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clipboard manager with advanced features.
> More information: <https://hluk.github.io/CopyQ/>.

#### Launch CopyQ to store clipboard history:
```shell
copyq
```
#### Show current clipboard content:
```shell
copyq clipboard
```
#### Insert raw text into the clipboard history:
```shell
copyq add -- {{text1}} {{text2}} {{text3}}
```
#### Insert text containing escape sequences ('\n', '\t') into the clipboard history:
```shell
copyq add {{firstline\nsecondline}}
```
#### Print the content of the first 3 items in the clipboard history:
```shell
copyq read 0 1 2
```
#### Copy a file's contents into the clipboard:
```shell
copyq copy < {{file.txt}}
```
#### Copy a JPEG image into the clipboard:
```shell
copyq copy image/jpeg < {{image.jpg}}
```
{% endraw %}