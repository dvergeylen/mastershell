---
layout: default
title: "textutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="textutil">
  <a href="/en/osx/textutil.html">textutil</a> <a href="#textutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Used to manipulate text files of various formats.

#### Display information about `foo.rtf`:
```shell
textutil -info {{foo.rtf}}
```
#### Convert `foo.rtf` into `foo.html`:
```shell
textutil -convert {{html}} {{foo.rtf}}
```
#### Convert rich text to normal text:
```shell
textutil {{foo.rtf}} -convert {{txt}}
```
#### Convert `foo.txt` into `foo.rtf`, using Times 10 for the font:
```shell
textutil -convert {{rtf}} -font {{Times}} -fontsize {{10}} {{foo.txt}}
```
#### Load all RTF files in the current directory, concatenates their contents, and writes the result out as `index.html` with the HTML title set to "Several Files":
```shell
textutil -cat {{html}} -title "Several Files" -output {{index.html}} *.rtf
```
{% endraw %}