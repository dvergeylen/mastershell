---
layout: default
title: "vimdiff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vimdiff">
  <a href="/en/common/vimdiff.html">vimdiff</a> <a href="#vimdiff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open up two or more files in vim and show the differences between them.
> See also `vim`.
> More information: <https://www.vim.org>.

#### Open two files and show the differences:
```shell
vimdiff {{file1}} {{file2}}
```
#### Move the cursor to the window on the left|right:
```shell
Ctrl + w {{h|l}}
```
#### Jump to the next difference:
```shell
[c
```
#### Jump to the previous difference:
```shell
]c
```
#### Copy the highlighted difference from the other window to the current window:
```shell
do
```
#### Copy the highlighted difference from the current window to the other window:
```shell
dp
```
#### Update all highlights and folds:
```shell
:diffupdate
```
#### Toggle the highlighted code fold:
```shell
za
```
{% endraw %}