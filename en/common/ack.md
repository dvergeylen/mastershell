---
layout: default
title: "ack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ack">
  <a href="/en/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A search tool like grep, optimized for developers.
> See also: `rg`, which is much faster.
> More information: <https://beyondgrep.com/documentation>.

#### Search for files containing a string or regular expression in the current directory recursively:
```shell
ack "{{search_pattern}}"
```
#### Search for a case-insensitive pattern:
```shell
ack --ignore-case "{{search_pattern}}"
```
#### Search for lines matching a pattern, printing [o]nly the matched text and not the rest of the line:
```shell
ack -o "{{search_pattern}}"
```
#### Limit search to files of a specific type:
```shell
ack --type={{ruby}} "{{search_pattern}}
```
#### Do not search in files of a specific type:
```shell
ack --type=no{{ruby}} "{{search_pattern}}
```
#### Count the total number of matches found:
```shell
ack --count --no-filename "{{search_pattern}}"
```
#### Print the file names and the number of matches for each file only:
```shell
ack --count --files-with-matches "{{search_pattern}}"
```
#### List all values that can be used with `--type`:
```shell
ack --help-types
```
{% endraw %}