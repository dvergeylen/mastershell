---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/en/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print and concatenate files.
> A `cat` clone with syntax highlighting and Git integration.
> More information: <https://github.com/sharkdp/bat>.

#### Print the contents of a file to the standard output:
```shell
bat {{file}}
```
#### Concatenate several files into the target file:
```shell
bat {{file1}} {{file2}} > {{target_file}}
```
#### Append several files into the target file:
```shell
bat {{file1}} {{file2}} >> {{target_file}}
```
#### Number all output lines:
```shell
bat -n {{file}}
```
#### Syntax highlight a json file:
```shell
bat --language json {{file.json}}
```
#### Display all supported languages:
```shell
bat --list-languages
```
{% endraw %}