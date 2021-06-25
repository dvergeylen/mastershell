---
layout: default
title: "seq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="seq">
  <a href="/en/common/seq.html">seq</a> <a href="#seq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Output a sequence of numbers to stdout.
> More information: <https://www.gnu.org/software/coreutils/seq>.

#### Sequence from 1 to 10:
```shell
seq 10
```
#### Every 3rd number from 5 to 20:
```shell
seq 5 3 20
```
#### Separate the output with a space instead of a newline:
```shell
seq -s " " 5 3 20
```
#### Format output width to a minimum of 4 digits padding with zeros as necessary:
```shell
seq -f "%04g" 5 3 20
```
{% endraw %}