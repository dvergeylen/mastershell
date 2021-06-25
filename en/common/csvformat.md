---
layout: default
title: "csvformat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvformat">
  <a href="/en/common/csvformat.html">csvformat</a> <a href="#csvformat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert a CSV file to a custom output format.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvformat.html>.

#### Convert to a tab-delimited file (TSV):
```shell
csvformat -T {{data.csv}}
```
#### Convert delimiters to a custom character:
```shell
csvformat -D "{{custom_character}}" {{data.csv}}
```
#### Convert line endings to carriage return (^M) + line feed:
```shell
csvformat -M "{{\r\n}}" {{data.csv}}
```
#### Minimize use of quote characters:
```shell
csvformat -U 0 {{data.csv}}
```
#### Maximize use of quote characters:
```shell
csvformat -U 1 {{data.csv}}
```
{% endraw %}