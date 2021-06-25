---
layout: default
title: "pbcopy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pbcopy">
  <a href="/en/osx/pbcopy.html">pbcopy</a> <a href="#pbcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Place standard output in the clipboard.

#### Place the contents of a file in the clipboard:
```shell
pbcopy < {{file}}
```
#### Place the results of a command in the clipboard:
```shell
find . -type t -name "*.png" | pbcopy
```
{% endraw %}