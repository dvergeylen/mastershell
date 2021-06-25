---
layout: default
title: "yank"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yank">
  <a href="/en/osx/yank.html">yank</a> <a href="#yank"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read input from stdin and display a selection interface that allows a field to be selected and copied to the clipboard.

#### Yank using the default delimiters (\f, \n, \r, \s, \t):
```shell
{{sudo dmesg}} | yank
```
#### Yank an entire line:
```shell
{{sudo dmesg}} | yank -l
```
#### Yank using a specific delimiter:
```shell
{{echo hello=world}} | yank -d {{=}}
```
#### Only yank fields matching a specific pattern:
```shell
{{ps ux}} | yank -g "{{[0-9]+}}"
```
{% endraw %}