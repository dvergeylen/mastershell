---
layout: default
title: "ptx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ptx">
  <a href="/en/linux/ptx.html">ptx</a> <a href="#ptx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a permuted index of words from one or more text files.
> More information: <https://www.gnu.org/software/coreutils/ptx>.

#### Generate a permuted index where the first field of each line is an index reference:
```shell
ptx --references {{path/to/file}}
```
#### Generate a permuted index with automatically generated index references:
```shell
ptx --auto-reference {{path/to/file}}
```
#### Generate a permuted index with a fixed width:
```shell
ptx --width={{width_in_columns}} {{path/to/file}}
```
#### Generate a permuted index with a list of filtered words:
```shell
ptx --only-file={{path/to/filter}} {{path/to/file}}
```
#### Generate a permuted index with SYSV-style behaviors:
```shell
ptx --traditional {{path/to/file}}
```
{% endraw %}