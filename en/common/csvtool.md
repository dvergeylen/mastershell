---
layout: default
title: "csvtool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvtool">
  <a href="/en/common/csvtool.html">csvtool</a> <a href="#csvtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to filter and extract data from CSV formatted sources.
> More information: <https://github.com/maroofi/csvtool>.

#### Extract the second column from a CSV file:
```shell
csvtool --column {{2}} {{path/to/file.csv}}
```
#### Extract the second and fourth columns from a CSV file:
```shell
csvtool --column {{2,4}} {{path/to/file.csv}}
```
#### Extract lines from a CSV file where the second column exactly matches 'Foo':
```shell
csvtool --column {{2}} --search '{{^Foo$}}' {{path/to/file.csv}}
```
#### Extract lines from a CSV file where the second column starts with 'Bar':
```shell
csvtool --column {{2}} --search '{{^Bar}}' {{path/to/file.csv}}
```
#### Find lines in a CSV file where the second column ends with 'Baz' and then extract the third and sixth columns:
```shell
csvtool --column {{2}} --search '{{Baz$}}' {{path/to/file.csv}} | csvtool --no-header --column {{3,6}}
```
{% endraw %}