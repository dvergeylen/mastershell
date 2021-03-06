---
layout: default
title: "repren"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="repren">
  <a href="/en/common/repren.html">repren</a> <a href="#repren"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multi-pattern string replacement and file renaming tool.
> More information: <https://github.com/jlevy/repren>.

#### Do a dry-run renaming a directory of pngs with a literal string replacement:
```shell
repren --dry-run --rename --literal --from '{{find_string}}' --to '{{replacement_string}}' {{*.png}}
```
#### Do a dry-run renaming a directory of jpegs with a regular expression:
```shell
repren --rename --dry-run --from '{{regular_expression}}' --to '{{replacement_string}}' {{*.jpg}} {{*.jpeg}}
```
#### Do a find-and-replace on the contents of a directory of csv files:
```shell
repren --from '{{([0-9]+) example_string}}' --to '{{replacement_string \1}}' {{*.csv}}
```
#### Do both a find-and-replace and a rename operation at the same time, using a pattern file:
```shell
repren --patterns {{path/to/patfile.ext}} --full {{*.txt}}
```
#### Do a case-insensitive rename:
```shell
repren --rename --insensitive --patterns {{path/to/patfile.ext}} *
```
{% endraw %}