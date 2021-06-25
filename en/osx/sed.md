---
layout: default
title: "sed"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sed">
  <a href="/en/osx/sed.html">sed</a> <a href="#sed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit text in a scriptable manner.
> More information: <https://ss64.com/osx/sed.html>.

#### Replace the first occurrence of a string in a file, and print the result:
```shell
sed 's/{{find}}/{{replace}}/' {{filename}}
```
#### Replace all occurrences of an extended regular expression in a file:
```shell
sed -E 's/{{regular_expression}}/{{replace}}/g' {{filename}}
```
#### Replace all occurrences of a string [i]n a file, overwriting the file (i.e. in-place):
```shell
sed -i '' 's/{{find}}/{{replace}}/g' {{filename}}
```
#### Replace only on lines matching the line pattern:
```shell
sed '/{{line_pattern}}/s/{{find}}/{{replace}}/' {{filename}}
```
#### Print only text between n-th line till the next empty line:
```shell
sed -n '{{line_number}},/^$/p' {{filename}}
```
#### Apply multiple find-replace expressions to a file:
```shell
sed -e 's/{{find}}/{{replace}}/' -e 's/{{find}}/{{replace}}/' {{filename}}
```
#### Replace separator / by any other character not used in the find or replace patterns, e.g., #:
```shell
sed 's#{{find}}#{{replace}}#' {{filename}}
```
#### [d]elete the line at the specific line number [i]n a file, overwriting the file:
```shell
sed -i '' '{{line_number}}d' {{filename}}
```
{% endraw %}