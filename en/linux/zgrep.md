---
layout: default
title: "zgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zgrep">
  <a href="/en/linux/zgrep.html">zgrep</a> <a href="#zgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Grep text patterns from files within compressed file (equivalent to grep -Z).

#### Grep a pattern in a compressed file (case-sensitive):
```shell
zgrep {{pattern}} {{path/to/compressed/file}}
```
#### Grep a pattern in a compressed file (case-insensitive):
```shell
zgrep -i {{pattern}} {{path/to/compressed/file}}
```
#### Output count of lines containing matched pattern in a compressed file:
```shell
zgrep -c {{pattern}} {{path/to/compressed/file}}
```
#### Display the lines which don’t have the pattern present (Invert the search function):
```shell
zgrep -v {{pattern}} {{path/to/compressed/file}}
```
#### Grep a compressed file for multiple patterns:
```shell
zgrep -e "{{pattern_1}}" -e "{{pattern_2}}" {{path/to/compressed/file}}
```
#### Use extended regular expressions (supporting `?`, `+`, `{}`, `()` and `|`):
```shell
zgrep -E {{regular_expression}} {{path/to/file}}
```
#### Print 3 lines of [C]ontext around, [B]efore, or [A]fter each match:
```shell
zgrep -{{C|B|A}} {{3}} {{pattern}} {{path/to/compressed/file}}
```
{% endraw %}