---
layout: default
title: "sed"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sed">
  <a href="/en/common/sed.html">sed</a> <a href="#sed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit text in a scriptable manner.
> More information: <https://man.archlinux.org/man/sed.1>.

#### Replace the first occurrence of a regular expression in each line of a file, and print the result:
```shell
sed 's/{{regular_expression}}/{{replace}}/' {{filename}}
```
#### Replace all occurrences of an extended regular expression in a file, and print the result:
```shell
sed -r 's/{{regular_expression}}/{{replace}}/g' {{filename}}
```
#### Replace all occurrences of a string in a file, overwriting the file (i.e. in-place):
```shell
sed -i 's/{{find}}/{{replace}}/g' {{filename}}
```
#### Replace only on lines matching the line pattern:
```shell
sed '/{{line_pattern}}/s/{{find}}/{{replace}}/' {{filename}}
```
#### Delete lines matching the line pattern:
```shell
sed '/{{line_pattern}}/d' {{filename}}
```
#### Print the first 11 lines of a file:
```shell
sed 11q {{filename}}
```
#### Apply multiple find-replace expressions to a file:
```shell
sed -e 's/{{find}}/{{replace}}/' -e 's/{{find}}/{{replace}}/' {{filename}}
```
#### Replace separator `/` by any other character not used in the find or replace patterns, e.g., `#`:
```shell
sed 's#{{find}}#{{replace}}#' {{filename}}
```
{% endraw %}