---
layout: default
title: "csvsort"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvsort">
  <a href="/en/common/csvsort.html">csvsort</a> <a href="#csvsort"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sorts CSV files.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvsort.html>.

#### Sort a CSV file by column 9:
```shell
csvsort -c {{9}} {{data.csv}}
```
#### Sort a CSV file by the "name" column in descending order:
```shell
csvsort -r -c {{name}} {{data.csv}}
```
#### Sort a CSV file by column 2, then by column 4:
```shell
csvsort -c {{2,4}} {{data.csv}}
```
#### Sort a CSV file without inferring data types:
```shell
csvsort --no-inference -c {{columns}} {{data.csv}}
```
{% endraw %}