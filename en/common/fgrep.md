---
layout: default
title: "fgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fgrep">
  <a href="/en/common/fgrep.html">fgrep</a> <a href="#fgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Matches patterns in files.
> Supports simple patterns and regular expressions.
> More information: <https://manned.org/fgrep>.

#### Search for an exact string in a file:
```shell
fgrep {{search_string}} {{path/to/file}}
```
#### Search only lines that match entirely in files:
```shell
fgrep -x {{path/to/file1}} {{path/to/file2}}
```
#### Count the number of lines that match the given string in a file:
```shell
fgrep -c {{search_string}} {{path/to/file}}
```
#### Show the line number in the file along with the line matched:
```shell
fgrep -n {{search_string}} {{path/to/file}}
```
#### Display all lines except those that contain the given regular expression:
```shell
fgrep -v {{regular_expression}} {{path/to/file}}
```
#### Display filenames whose content matches the regular expression at least once:
```shell
fgrep -l {{regular_expression}} {{path/to/file1}} {{path/to/file2}}
```
{% endraw %}