---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/en/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print and concatenate files.
> More information: <https://www.gnu.org/software/coreutils/cat>.

#### Print the contents of a file to the standard output:
```shell
cat {{file}}
```
#### Concatenate several files into the target file:
```shell
cat {{file1}} {{file2}} > {{target_file}}
```
#### Append several files into the target file:
```shell
cat {{file1}} {{file2}} >> {{target_file}}
```
#### Number all output lines:
```shell
cat -n {{file}}
```
#### Display non-printable and whitespace characters (with `M-` prefix if non-ASCII):
```shell
cat -v -t -e {{file}}
```
{% endraw %}