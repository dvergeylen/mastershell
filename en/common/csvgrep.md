---
layout: default
title: "csvgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvgrep">
  <a href="/en/common/csvgrep.html">csvgrep</a> <a href="#csvgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Filter CSV rows with string and pattern matching.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvgrep.html>.

#### Find rows that have a certain string in column 1:
```shell
csvgrep -c {{1}} -m {{string_to_match}} {{data.csv}}
```
#### Find rows in which columns 3 or 4 match a certain regular expression:
```shell
csvgrep -c {{3,4}} -r {{regular_expression}} {{data.csv}}
```
#### Find rows in which the "name" column does NOT include the string "John Doe":
```shell
csvgrep -i -c {{name}} -m "{{John Doe}}" {{data.csv}}
```
{% endraw %}