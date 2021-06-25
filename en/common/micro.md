---
layout: default
title: "micro"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="micro">
  <a href="/en/common/micro.html">micro</a> <a href="#micro"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Micro is a modern and intuitive terminal-based text editor.
> You can use your keyboard, but also your mouse to navigate and/or select text.
> More information: <https://micro-editor.github.io>.

#### Open a file:
```shell
micro {{file}}
```
#### Cut the entire line:
```shell
Ctrl + K
```
#### Search for a pattern in the file (press `Ctrl + N`/`Ctrl + P` to go to next/previous match):
```shell
Ctrl + F "{{pattern}}" <Enter>
```
#### Execute a command:
```shell
Ctrl + E {{command}} <Enter>
```
#### Perform a substitution in the whole file:
```shell
Ctrl + E replaceall "{{pattern}}" "{{replacement}}" <Enter>
```
#### Quit:
```shell
Ctrl + Q
```
{% endraw %}