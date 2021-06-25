---
layout: default
title: "csvstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvstat">
  <a href="/en/common/csvstat.html">csvstat</a> <a href="#csvstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print descriptive statistics for all columns in a CSV file.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvstat.html>.

#### Show all stats for all columns:
```shell
csvstat {{data.csv}}
```
#### Show all stats for columns 2 and 4:
```shell
csvstat -c {{2,4}} {{data.csv}}
```
#### Show sums for all columns:
```shell
csvstat --sum {{data.csv}}
```
#### Show the max value length for column 3:
```shell
csvstat -c {{3}} --len {{data.csv}}
```
#### Show the number of unique values in the "name" column:
```shell
csvstat -c {{name}} --unique {{data.csv}}
```
{% endraw %}