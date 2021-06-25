---
layout: default
title: "xed"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xed">
  <a href="/en/osx/xed.html">xed</a> <a href="#xed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opens files for editing in Xcode.

#### Open file in Xcode:
```shell
xed {{file1}}
```
#### Open file(s) in Xcode, create if it doesn't exist:
```shell
xed -c {{filename1}}
```
#### Open a file in Xcode and jump to line number 75:
```shell
xed -l 75 {{filename}}
```
{% endraw %}