---
layout: default
title: "csvcut"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvcut">
  <a href="/en/common/csvcut.html">csvcut</a> <a href="#csvcut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Filter and truncate CSV files. Like Unix's `cut` command, but for tabular data.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvcut.html>.

#### Print indices and names of all columns:
```shell
csvcut -n {{data.csv}}
```
#### Extract the first and third columns:
```shell
csvcut -c {{1,3}} {{data.csv}}
```
#### Extract all columns **except** the fourth one:
```shell
csvcut -C {{4}} {{data.csv}}
```
#### Extract the columns named "id" and "first name" (in that order):
```shell
csvcut -c {{id,"first name"}} {{data.csv}}
```
{% endraw %}