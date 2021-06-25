---
layout: default
title: "sensible-editor"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sensible-editor">
  <a href="/en/linux/sensible-editor.html">sensible-editor</a> <a href="#sensible-editor"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open the default editor.

#### Open a file in the default editor:
```shell
sensible-editor {{file}}
```
#### Open a file in the default editor, with the cursor at the end of the file:
```shell
sensible-editor + {{file}}
```
#### Open a file in the default editor, with the cursor at the beginning of line 10:
```shell
sensible-editor +10 {{file}}
```
#### Open 3 files in vertically split editor windows at the same time:
```shell
sensible-editor -O3 {{file_1}} {{file_2}} {{file_3}}
```
{% endraw %}