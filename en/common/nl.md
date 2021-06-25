---
layout: default
title: "nl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nl">
  <a href="/en/common/nl.html">nl</a> <a href="#nl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility for numbering lines, either from a file, or from standard input.
> More information: <https://www.gnu.org/software/coreutils/nl>.

#### Number non-blank lines in a file:
```shell
nl {{file}}
```
#### Read from standard output:
```shell
cat {{file}} | nl {{options}} -
```
#### Number only the lines with printable text:
```shell
nl -t {{file}}
```
#### Number all lines including blank lines:
```shell
nl -b a {{file}}
```
#### Number only the body lines that match a basic regular expression (BRE) pattern:
```shell
nl -b p'FooBar[0-9]' {{file}}
```
{% endraw %}