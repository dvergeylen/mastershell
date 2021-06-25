---
layout: default
title: "wc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wc">
  <a href="/en/common/wc.html">wc</a> <a href="#wc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Count lines, words, or bytes.
> More information: <https://www.gnu.org/software/coreutils/wc>.

#### Count lines in file:
```shell
wc -l {{file}}
```
#### Count words in file:
```shell
wc -w {{file}}
```
#### Count characters (bytes) in file:
```shell
wc -c {{file}}
```
#### Count characters in file (taking multi-byte character sets into account):
```shell
wc -m {{file}}
```
#### Use standard input to count lines, words and characters (bytes) in that order:
```shell
{{find .}} | wc
```
{% endraw %}