---
layout: default
title: "expand"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="expand">
  <a href="/en/common/expand.html">expand</a> <a href="#expand"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert tabs to spaces.
> More information: <https://www.gnu.org/software/coreutils/expand>.

#### Convert tabs in each file to spaces, writing to standard output:
```shell
expand {{file}}
```
#### Convert tabs to spaces, reading from standard input:
```shell
expand
```
#### Do not convert tabs after non blanks:
```shell
expand -i {{file}}
```
#### Have tabs a certain number of characters apart, not 8:
```shell
expand -t={{number}} {{file}}
```
#### Use a comma separated list of explicit tab positions:
```shell
expand -t={{1,4,6}}
```
{% endraw %}