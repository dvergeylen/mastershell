---
layout: default
title: "aspell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aspell">
  <a href="/en/linux/aspell.html">aspell</a> <a href="#aspell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interactive spell checker.

#### Spell check a single file:
```shell
aspell check {{path/to/file}}
```
#### List misspelled words from standard input:
```shell
cat {{file}} | aspell list
```
#### Show available dictionary languages:
```shell
aspell dicts
```
#### Run aspell with different language (takes two letter ISO 639 language code):
```shell
aspell --lang={{cs}}
```
#### List misspelled words from standard input and ignore words from personal word list:
```shell
cat {{file}} | aspell --personal={{personal-word-list.pws}} {{list}}
```
{% endraw %}